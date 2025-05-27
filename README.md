Certainly! Below is the entire **`README.md`** file for your project:

````markdown
# React-Crop-Rotation

A simple React application that allows users to crop and rotate images with interactive UI. It uses the `react-image-crop` library for cropping and a custom hook for rotating images.

## Features

- **Image Cropping**: Crop images freely or using a fixed aspect ratio.
- **Image Rotation**: Rotate images in 90-degree increments.
- **Live Preview**: See the result of the crop and rotation in real-time.
- **Image Save**: After cropping, save the cropped image.

## Live Demo

You can try a live demo of this project on [CodeSandbox](https://codesandbox.io/p/sandbox/2tfygx).

## Installation

To get started with this project locally, follow these steps:

### 1. Clone the repository

```bash
git clone https://github.com/your-username/react-crop-rotation.git
````

### 2. Navigate to the project folder

```bash
cd react-crop-rotation
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the application

```bash
npm start
```

This will start the React development server and open the app in your browser.

## Usage

### Crop an Image

* Import the `ReactImageCrop` component into your app.
* Pass the image URL and cropping options as props.
* Use the rotation feature to adjust the orientation of the image.
* After cropping, you can save the cropped image as a new file.

```jsx
<ReactImageCrop
  src="path-to-your-image.jpg"
  crop={crop}
  onChange={handleCropChange}
  rotation={rotateDeg}
  onComplete={handleCropComplete}
/>
```

### Rotate the Image

* Use the buttons to rotate the image in 90-degree increments.
* Rotation will be applied immediately, and the cropped image will adjust accordingly.

```jsx
<Button onClick={() => setRotateDeg((r) => (r + 90) % 360)}>
  Rotate Left
</Button>
<Button onClick={() => setRotateDeg((r) => (r - 90) % 360)}>
  Rotate Right
</Button>
```

## Custom Hook for Image Rotation

The rotation logic is encapsulated in a custom hook `useRotateImage`. It handles the image rotation and provides the rotated image URL.

```js
const rotatedImage = useRotateImage(imageSrc, rotateDeg);
```

## Tech Stack

* React
* react-image-crop
* Ant Design (for UI components)
* HTML5 Canvas (for image rotation)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by \[Your Name]

```

---

### Key Sections Explained:
- **Project Overview**: Provides a short summary of the project’s functionality.
- **Live Demo**: Link to the working demo of the project on CodeSandbox.
- **Installation Instructions**: How to set up and run the project locally.
- **Usage Instructions**: Code examples and explanations of how to use the cropping and rotation features.
- **Tech Stack**: A list of the libraries and technologies used in the project.
- **License**: Details on the licensing of the project (MIT in this case).
- **Credits**: Optionally, you can credit yourself as the author at the end.

Feel free to modify the file to include more details as necessary or adjust the style! Let me know if you need any changes or additions.
```
