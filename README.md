# QRCode Generator
#### This is the python file for generate QRCode by using framework "qrcode".
##### I'm learn this skill from this website: https://www.geeksforgeeks.org/generate-qr-code-using-qrcode-in-python/

##### Importing library
```
import qrcode
```
* Data to be encoded
```
data = 'QR Code using make() function'
```
* Encoding data using make() function
```
img = qrcode.make(data)
```
* Saving as an image file
```
img.save('MyQRCode1.png')
```



* Full code
```
  # Importing library
import qrcode
 
# Data to encode
data = "GeeksforGeeks"
 
# Creating an instance of QRCode class
qr = qrcode.QRCode(version = 1,
                   box_size = 10,
                   border = 5)
 
# Adding data to the instance 'qr'
qr.add_data(data)
 
qr.make(fit = True)
img = qr.make_image(fill_color = 'red',
                    back_color = 'white')
 
img.save('MyQRCode2.png')
```
