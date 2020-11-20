# RN Camera example with Expo


Prototype to capture image using camera. I usually use Expo and if you're not using then you will have to uninstall expo-camera and expo-permissions, instad install [React Native Camera](https://github.com/react-native-camera/react-native-camera). Both works the same way.

On button click picture will be taken and you can find the console log as well.

```javascript
    const __takePicture = async () => {
        const photo = await camera.takePictureAsync()
        console.log('click', photo)
        setPreviewVisible(true)
        //setStartCamera(false)
        setCapturedImage(photo)
    }
```

The above function in app.js, you can find the console.log. Which you can save it in an state array using useState(). Object contains the URI for the imae path and Height and Width of the image.

Further more, run a loop of the array and append the images in UI