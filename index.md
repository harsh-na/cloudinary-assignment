title: Cloudinary uploader using Node.js
layout: page

# Welcome to Cloudinary uploader using Node.js

Upload files to your cloudinary account using Node.js and the [Cloudinary.js](https://www.npmjs.com/package/cloudinary) library.
In [this](https://github.com/RisoriTofa/Cloudinary-uploader-Node.js) repository, you will find code that will enable you to easily upload your images to Cloudinary. It is under MIT License. You can clone and modify it for your use.
You can use it as a template for your project as you would like.

## Table of Content

- [Folder Structure](#Folder-Structure)
- [How the project will run](#How-the-project-will-run)
- [Clone the repository](#Clone-the-repository)
- [Install the dependencies](#Install-the-dependencies)
- [Configuring package.json](#Configuring-package.json)
- [Configure "_.env_" file](#Configure-"_.env_"-file)
- [Run the project](#Run-the-project)
- [Output](#Output)

### Folder Structure

The folder structure will be as shown below:

> Cloudinary-uploader (Root Directory)
>
> > node_modules (folder)
> >
> > .env (file)
> >
> > index.js (file)
> >

### How the project will run

The code when executed will use the cloudinary.js library to upload the files to the cloudinary account using the credentials stored in the "_.env_" file. It shall then return a response both on the web browser and terminal.

### Clone the repository

Clone [this](https://github.com/RisoriTofa/Cloudinary-uploader-Node.js) repository on your machine.

### Install the dependencies

The node libraries required for this tutorial include:

- nodemon
- cloudinary
- formidable
- dotenv
- express

In the integrated terminal, run the following command to install the above packages all at once:

```node.js
npm i nodemon cloudinary dotenv formidable express
```
#### Configuring package.json

Now open the "package.json" file and configure it so that you can start the application using nodemon. Under the scripts, add the "dev" and "start" configurations. The code should look as follows:

```json
{
    "name": "Cloudinary-uploader-Node.js",
    "version": "1.0.0",
    "description": "In this repository, you will find code that will enable you to easily upload your images to Cloudinary. It is under MIT License. You can clone and modify it for your use.",
    "main": "index.js",
    "scripts": {
        "start": "node index.js",
        "dev": "nodemon index.js",
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/RisoriTofa/Cloudinary-uploader-Node.js.git"
    },
    "keywords": [],
    "author": "",
    "license": "ISC",
    "bugs": {
        "url": "https://github.com/RisoriTofa/Cloudinary-uploader-Node.js/issues"
    },
    "homepage": "https://github.com/RisoriTofa/Cloudinary-uploader-Node.js#readme",
    "dependencies": {
        "cloudinary": "^1.25.1",
        "dotenv": "^8.2.0",
        "express": "^4.17.1",
        "formidable": "^1.2.2",
        "nodemon": "^2.0.7"
    }
}
```

### Configure "_.env_" file

Add your credentials to the "_.env_" file and save it.

### Run the project

Before running the code, make sure that MongoDB is running in the background.

In your integrated terminal, run the following command:
`
nodemon run dev
`

## Output

**Main Webpage**
![Main Webpage](uploader-landing-page.png?raw=true "Uploader Webpage")

**Recieved files Webpage**
![Recieved files Webpage](recieved-file-cloudinary-Node.js.png?raw=true "Uploader Webpage")

And that is all!
Feel free to contribute to the repository as you see well through [discussions](https://github.com/RisoriTofa/Cloudinary-uploader-Node.js/discussions) or add new [issues](https://github.com/RisoriTofa/Cloudinary-uploader-Node.js/issues).

_Author: **RisoriTofa**_
