# DetectNumber: License Plate Detection and Recognition  

**DetectNumber** is a tool that detects and crops license plates from images, aligns tilted plates, and performs recognition of alphanumeric characters (36 classes: 0-9, A-Z) from the detected data.  

![License Plate Detection Demo](https://via.placeholder.com/800x400?text=Add+Your+Image+Here)  

## Features  

- **License Plate Detection**: Automatically detects license plates in an image using an ANPR (Automatic Number Plate Recognition) tool.  
- **Image Cropping**: Crops detected license plates and saves them in a directory for further processing.  
- **Alignment Correction**: Corrects tilted plates, ensuring proper alignment for recognition.  
- **Character Recognition**: Recognizes and classifies 36 alphanumeric characters (0-9, A-Z) from license plates.  

## How It Works  

1. **Detection**: The ANPR tool identifies license plates in the input image.  
2. **Cropping**: Detected license plates are cropped and stored in the designated directory.  
3. **Alignment**: Tilted images are automatically corrected for better readability.  
4. **Recognition**: A trained model recognizes alphanumeric characters from the cropped and aligned license plate images.  

## How to Use  

1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/yourusername/detectnumber.git  
   cd detectnumber  
   ```  

2. **Install Dependencies**:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. **Run Detection and Cropping**:  
   Add your images to the `input/` directory and execute the script:  
   ```bash  
   python detect_and_crop.py  
   ```  

4. **Character Recognition**:  
   Use the recognition script to classify characters:  
   ```bash  
   python recognize_characters.py  
   ```  

## File Structure  

```
detectnumber/  
│  
├── input/                     # Directory to add input images  
├── output/                    # Directory for cropped license plates  
├── models/                    # Pre-trained model for character recognition  
│   ├── license_recognition.pkl  
│  
├── detect_and_crop.py         # Script for detection and cropping  
├── recognize_characters.py    # Script for character recognition  
├── requirements.txt           # List of dependencies  
├── README.md                  # Project documentation  
└── LICENSE                    # License information  
```  

## Results  

- Cropped license plates are saved in the `output/` directory.  
- Recognized characters are displayed on the terminal or saved in a file.  

## Dependencies  

- Python 3.x  
- OpenCV  
- NumPy  
- TensorFlow or PyTorch (for recognition model)  
- Matplotlib  

Install all dependencies using:  
```bash  
pip install -r requirements.txt  
```  

## Contributing  

Contributions are welcome! Fork the repository, implement your improvements, and submit a pull request.  

## License  

This project is licensed under the MIT License.  


