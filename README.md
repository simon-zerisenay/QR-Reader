<div align="center">
 
# Qr-code-reader-react-native-expo-
  <a href="https://github.com/simon-zerisenay/QR-Reader" target="_blank">
    <img src="https://github.com/simon-zerisenay/simon-zerisenay/blob/main/QRREADER.png"  padding="20" height="170" width="200" alt="twitter logo"  />
  </a> 
 
 </div>  
This is a React Native component that uses the expo-barcode-scanner package to scan barcodes using the device's camera. The component has three states, hasPermission, scanned, and setScanned. The hasPermission state is used to determine if the app has permission to use the device's camera. The scanned state is used to determine if a barcode has been scanned. The setScanned state is used to update the scanned state when a barcode is scanned or when the user taps the "Tap to Scan Again" button.
   
The component has a useEffect hook that runs when the component mounts. It requests camera permission from the user and updates the hasPermission state accordingly.

The handleBarCodeScanned function is called when a barcode is scanned. It updates the scanned state to true and displays an alert with the barcode's type and data.
 
The component renders a View component that contains a BarCodeScanner component from the expo-barcode-scanner package. The onBarCodeScanned prop of the BarCodeScanner component is set to undefined if the scanned state is true. This prevents the handleBarCodeScanned function from being called multiple times if the user holds the camera over the barcode for too long. The Button component is only displayed if the scanned state is true and the user can tap it to scan again.
 
The StyleSheet component is used to define the styles for the container style rule. It defines a container that takes up the full height and width of the screen and centers its contents vertically. 
 
 
 
