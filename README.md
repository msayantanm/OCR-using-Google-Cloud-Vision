# OCR-using-Google-Cloud-Vision
This uses Google's CloudVision API to extract text from scanned images.  

The main objective is to extract the text from an image, which can be done through various OCR engines, and Google's CloudVision(GCV) is one of them. There are many open-source tools available, the most popular one being PyTesseract OCR for python. The main advantage of GCV is that the handwritten entries are also being extracted pretty accurately, thanks to the powerful ML models to detect and extract text from images. 
The direct call to GCV works fine, but for elaborate documents like a form, we need some helper functions which format and gives the resulting text in each line, for you to further use anywhere as you like! Preprocessing the image, before the API call works wonders, as the gradient difference between the foreground and background helps the models pick up text, even in harsh conditions.


# Prerequisites
To run this project, you will need the following:

Google Cloud Platform (GCP) account: You will need a GCP account to enable and use the Cloud Vision API. Visit the GCP Console to create a new account or use an existing one.

Project setup: Create a new project in the GCP Console, or use an existing one. Enable the Cloud Vision API for your project.

API credentials: Generate API credentials (API key or service account key) to authenticate your requests to the Cloud Vision API. Store the credentials securely and make sure they are accessible to your application.

Programming language and environment: Choose a programming language and set up the necessary development environment. This project supports multiple programming languages, including Python, Java, and Node.js. Ensure that you have the required dependencies installed.

Images with text: Gather the images from which you want to extract text. The Cloud Vision API supports various image formats, including JPEG, PNG, and GIF.

# Getting Started
Clone or download the project repository to your local machine.

Install the required dependencies according to the chosen programming language. Refer to the official documentation for the specific programming language to set up the necessary dependencies.

Configure API credentials: Store your API credentials securely. If you are using an API key, ensure that it is set as an environment variable or configured in your code. If you are using a service account key, ensure that the JSON key file is stored securely and accessible to your application.  

Replace the placeholder images in the project with your own images or modify the code to load images from a different location.

Run the project: Execute the code to extract text from the images. Depending on the programming language, you may need to run a specific command or execute a script.  


# References
- Google Cloud Vision API documentation: [https://cloud.google.com/vision](https://cloud.google.com/vision/docs)
