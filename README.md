# Expo Image Component URL Encoding Issue

This repository demonstrates a bug where the Expo `Image` component fails to load images when the URL contains special characters (like spaces or accented characters).  The issue is that the URL is not properly URL-encoded, leading to the image request failing silently.

## Bug Reproduction

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app using Expo Go or EAS.
4. Observe that the image with the URL containing a space fails to load.  The console will show no errors related to the image loading failure.

## Solution

The solution involves URL-encoding the image URL before passing it to the `Image` component.  This ensures that special characters are properly handled by the server and the image is successfully loaded.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.