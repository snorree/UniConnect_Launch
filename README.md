# UniConnect

UniConnect is a platform connecting prospective university students with current students for consultations about university life and application processes.

## Environment Setup

The application uses environment variables to store sensitive information. Follow these steps to set up your local environment:

1. Create a `.env` file in the root directory of the project
2. Add the following variables to your `.env` file:

```
FORMSPREE_ENDPOINT=your_formspree_endpoint
```

Replace `your_formspree_endpoint` with your actual Formspree form ID.

## Running the Application

This is a static website that can be served from any web server. To run it locally:

1. Open the `Landing_Page.html` file in your browser
2. You can also use a local development server like:
   - [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension for VSCode
   - Python's built-in server: `python -m http.server`
   - Node.js http-server: `npx http-server`

## Security Notes

- The `.env` file contains sensitive information and is excluded from version control via `.gitignore`
- When deploying, make sure to set the environment variables on your hosting platform
- For local development, the application will fall back to default values if the `.env` file is not accessible

## Project Structure

- `Landing_Page.html` - The main landing page of the application
- `How_It_Works.html` - Information about how the service works
- `privacy_policy.html` - Privacy policy for the application
- `success.html` - Success page shown after form submission 