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
    "projects": [
        {
            "name": "Example project 1",
            "description": "Description of your project",
            "github": "https://github.com/you/project1",
            "liveDemo": "https://project1.com",
            "image": "project_photos/sample1.png"  //place project cover photos in that folder and set the path to it as shown or just paste the URL
        },
        {
            "name": "Example project 2",
            "description": "Description of your project",
            "github": "https://github.com/you/project2",
            "liveDemo": "https://project2.com",
            "image": "project_photos/sample2.png"
        },
        {
            "name": "Example project 3",
            "description": "Description of your project",
            "github": "https://github.com/you/project3",
            "liveDemo": "https://project3.com",
            "image": "project_photos/sample3.png"
        }
    ],
    "certifications": [
        {
            "name": "Example Azure Certification",
            "provider": "Microsoft"
        },
        {
            "name": "Example AWS Certification",
            "provider": "Amazon Web Services"
        },
        {
            "name": "Example Google Cloud Certification",
            "provider": "Google Cloud"
        }
    ],
    "articles": {
        "header": "Check out my recent articles on Dev.to!",
        "items": [
            {
                "title": "Getting Started with AWS Lambda (example article)",
                "url": "https://dev.to/jrandomArticle1",
                "cover": "article_cover_photos/getting-started-aws-lambda.png" //place article cover photos in that folder and set the path to it as shown or just paste the URL
            },
            {
                "title": "Deploying Apps on Azure (example article)",
                "url": "https://dev.to/randomArticle2",
                "cover": "article_cover_photos/deploying-apps-to-azure.png"  //place article cover photos in that folder and set the path to it as shown or just paste the URL
            }
        ]
    },
    "theme": "dark-blue", //theme color must be in this form: "light-color" or "dark-color" 
    "allowToggleDarkMode": true // enable this to spawn an icon that allows user to switch from dark to light mode in the top bar
}
```

Simply replace the placeholder values with your own information.

### 3. Add a Profile Picture
1. Place your profile picture inside the project folder.
2. Name the file **profilepic.png** (make sure it's in `.png` format).

### 4. Add Your Skills
1. Skills is a list (called an array). Each item in the array is of the form:
``` javascript {
    "platform": "Put cloud platform here"
    "list of skills": ["Put skill 1 here", "Skill 2 here"] // <--- make sure skills are separated by a comma
}
```
Replace all with skills you want to display. If you don't want to display skills yet, remove the content in skills and leave it as an empty array ([])
Your image will automatically appear on the portfolio page.

### 5. Add Certifications
To showcase your certifications, add entries under the `certifications` array in `data.json`. Leave as empty array if you don't want to display this yet. When you come back, refer to this example to use the right from. Remeber to use a comma to separate values!

#### Example:
```json
"certifications": [
    {
        "name": "AWS Certified Solutions Architect",
        "provider": "Amazon Web Services"
    },
]
```
Each certification will be displayed in the portfolio.

### 6. Add Articles
To include your blog articles, add entries under the `articles` array in `data.json`. Leave as empty array if you don't want to display this yet. When you come back, refer to this example to use the right from. Remeber to use a comma to separate values!

#### Example:
```json
"articles": [
    {
        "title": "Getting Started with AWS Lambda (example article)",
        "url": "https://dev.to/example-article",
        "cover": "article_cover_photos/aws-lambda.png"
    }, 
]
```
Each article will be displayed on the portfolio with its respective cover image. Store the article cover photo in the `article_cover_photo` folder and link it as such. Or if the image has a url, simply add that as the url value.


### 7 Open the Portfolio
Once you've updated your details, open the `index.html` file in your browser to see your personalized portfolio!
Tip: install liver server on VS code to dynamically see the updates

## Customization
- To change the theme color, modify the `theme` value in `data.json` (You can select between these: `blue`, `grey`, `red`, `violet`, `green`, `deep_yellow`, `orange`, `beige`, `magenta`, `blackGrey` ). The value must be in the form `dark-color` or `light-color` ex: `"theme": "light-red"`, or `"theme": "light-deepYellow"`, or even `light-blackGrey` (If this isn't done correctly, it will default to dark and / or blue.)

- Find a list of themes and even add more themes in the theme.js file

- Modify `styles.css` if you want to adjust the design further.

## Deployment
To publish your portfolio online, you can use GitHub Pages:
1. Upload your project to GitHub.
2. Go to **Settings** → **Pages**.
3. Set the **Source** to the `main` branch.
4. Your portfolio will be live at `https://yourusername.github.io/yourrepository/`.

---

## We will use this to practice setup of CI/CD

Enjoy your new cloud developer portfolio! 🚀

