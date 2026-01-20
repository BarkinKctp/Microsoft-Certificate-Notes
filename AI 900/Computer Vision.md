# COMPUTER VISION

## CNN (Convolutional Neural Network)

1. Images with known labels (for example, 0: apple, 1: banana, or 2: orange) are fed into the network to train the model.  
2. One or more layers of filters is used to extract features from each image as it is fed through the network. The filter kernels start with randomly assigned weights and generate arrays of numeric values called feature maps.  
3. The feature maps are flattened into a single dimensional array of feature values.  
4. The feature values are fed into a fully connected neural network.  
5. The output layer of the neural network uses a softmax or similar function to produce a result that contains a probability value for each possible class, for example `[0.2, 0.5, 0.3]`.

---

### Transformers

Transformers work by processing huge volumes of data, and encoding language tokens (representing individual words or phrases) as vector-based embeddings (arrays of numeric values). You can think of an embedding as representing a set of dimensions that each represent some semantic attribute of the token. The embeddings are created such that tokens that are commonly used in the same context are closer together dimensionally than unrelated words.

---

### Microsoft Florence model

---

## Azure AI Vision

- Image classification  
- Object detection  

---

## FACE RECOGNITION

### Applications for face detection, analysis, and recognition

- Security  
- Social Media  
- Intelligent Monitoring  
- Advertising  
- Missing Person  
- Identity Validation  

### Services

- Azure AI Vision, which offers face detection and some basic face analysis, such as returning the bounding box coordinates around an image.  
- Azure AI Video Indexer, which you can use to detect and identify faces in a video.  
- Azure AI Face, which offers pre-built algorithms that can detect, recognize, and analyze faces.  

---

## OPTICAL CHARACTER RECOGNITION (OCR)

---

=========================================================================

Modern image classification solutions are based on deep learning techniques.

Semantic segmentation provides the ability to classify individual pixels in an image depending on the object that they represent.

Facial detection provides the ability to detect and analyze human faces in an image, including identifying a person's age based on a photograph.  
Identifying a user requesting access to a laptop is done by taking images from the laptop’s webcam and using facial detection and recognition to identify the user requesting access.  
Employee access to a secure building can be achieved by using facial recognition.

---

### Image Classification

Image classification classifies images based on their contents.  
Image classification is part of computer vision that is concerned with the primary contents of an image.  
Image classification is part of computer vision and can be used to evaluate images from an X-ray machine to quickly classify specific bone fracture types.  
This helps improve diagnosis and treatment plans.  
An image classification model is trained to facilitate the categorizing of the bone fractures.

---

### Object Detection

Object detection provides the ability to generate bounding boxes identifying the locations of different types of vehicles in an image.  
Object detection can be used to evaluate traffic monitoring images to quickly classify specific vehicle types, such as car, bus, or cyclist.  
Identifying wildlife in an image is an example of a computer vision solution that uses object detection.  
Object detection can be used to track livestock animals, such as cows, to support their safety and welfare.  
Object detection is used to return identified objects in an image, such as a cat, person, or chair.

---

### OCR and Spatial Analysis

OCR and Spatial Analysis are part of the Azure AI Vision service.  
OCR provides the ability to detect and read text in images.  
It can be used to extract text from scanned medical records to produce a digital archive from paper-based documents.  
Extracting text from manuscripts is an example of a computer vision solution that uses optical character recognition (OCR).  
OCR is used to extract text and handwriting from images.  
It can be used to extract signatures for attendance purposes.

---

### Tagging and Categorization

Tagging involves associating an image with metadata that summarizes the attributes of the image.  
Detecting image types involves identifying clip art images or line drawings.  
Content organization involves identifying people or objects in photos and organizing them based on the identification.  
Categorizing involves associating the contents of an image with a limited set of categories.

---

### Face Operations

Face identification in the Azure AI Face service can address one-to-many matching of one face in an image to a set of faces in a secure repository.  
Face verification has the capability for one-to-one matching of a face in an image to a single face from a secure repository or a photo to verify whether they are the same individual.

- Face attributes  
- Find similar face  

---

The computer vision service eliminates the need for choosing, training, and evaluating a model by providing pre-trained models.  
To use computer vision, you must create an Azure resource.  
The use of computer vision involves inferencing.

Each phrase returned by an image description task of the Azure AI Vision includes the confidence score.  
An endpoint and a key must be provided to access the Azure AI Vision service.  
Bounding box coordinates are returned by services such as object detection, but not image description.

---
