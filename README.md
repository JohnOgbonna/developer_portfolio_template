# Cloud Developer Portfolio Template

This is a simple, customizable portfolio template for cloud developers, built using HTML, CSS, and JavaScript. It allows you to easily modify your personal information through a JSON file, making it accessible for non-coders.

## Features
- Editable personal details (name, contact info, bio, skills, blog links) via `data.json`
- Responsive design with customizable theme colors
- Simple setup with no coding required

## How to Use

### 1. Clone the Repository
If you're using GitHub, you can download this project to your computer.

#### Option 1: Using Git (Recommended)
1. Open a terminal (Command Prompt, PowerShell, or Terminal on Mac/Linux)
2. Run the following command:
   ```sh
   git clone https://github.com/yourusername/yourrepository.git
   ```
3. Navigate into the project folder:
   ```sh
   cd yourrepository
   ```

#### Option 2: Manual Download (Don't do this)
1. Go to the GitHub repository page.
2. Click the **Code** button and select **Download ZIP**.
3. Extract the ZIP file on your computer.

### 2. Modify Your Information

The portfolio is controlled by a simple JSON file (`data.json`). Open `data.json` in a text editor (such as Notepad, VS Code, or any text editor) and update the fields with your information.

#### Example Structure:
```json
{
    "name": "Your Name",
    "contact": {
        "email": "your.email@example.com",
        "devto": "https://dev.to/yourprofile",
        "linkedin": "https://linkedin.com/in/yourprofile",
        "github": "https://github.com/yourusername"
    },
    "title": "Cloud Developer",
    "description": "A passionate cloud developer with expertise in AWS, Azure, and Google Cloud.",
    "skills": [
        {
            "platform": "AWS",
            "list": ["EC2", "S3", "Lambda", "DynamoDB"]
        },
        {
            "platform": "Azure",
            "list": ["Azure Functions", "Blob Storage", "Cosmos DB"]
        },
        {
            "platform": "Google Cloud",
            "list": ["Cloud Functions", "Cloud Storage", "Firestore"]
        }
    ],
    "blogs": [
        {
            "title": "My First Blog Post",
            "url": "https://yourblog.com/my-first-post"
        }
    ],
    "theme": "blue"
}
```

Simply replace the placeholder values with your own information.

### 3. Add a Profile Picture
1. Place your profile picture inside the project folder.
2. Name the file **profilepic.png** (make sure it's in `.png` format).

Your image will automatically appear on the portfolio page.

### 4. Open the Portfolio
Once you've updated your details, open the `index.html` file in your browser to see your personalized portfolio!

## Customization
- To change the theme color, modify the `theme` value in `data.json` (options: `blue`, `grey`, `red`, `violet`, `dark green`, `deep yellow`).
- Modify `styles.css` if you want to adjust the design further.

## Deployment
To publish your portfolio online, you can use GitHub Pages:
1. Upload your project to GitHub.
2. Go to **Settings** → **Pages**.
3. Set the **Source** to the `main` branch.
4. Your portfolio will be live at `https://yourusername.github.io/yourrepository/`.

---

## We will setup CI/CD later

Enjoy your new cloud developer portfolio! 🚀

