# QRCode Generator
#### This is the python file for generate QRCode by using framework "qrcode".
##### I'm learn this skill from this website: https://www.geeksforgeeks.org/generate-qr-code-using-qrcode-in-python/

##### Importing library
```
import qrcode
```
##### Data to be encoded
```
data = 'QR Code using make() function'
```
##### Encoding data using make() function
```
img = qrcode.make(data)
```
##### Saving as an image file
```
img.save('MyQRCode1.png')
```

