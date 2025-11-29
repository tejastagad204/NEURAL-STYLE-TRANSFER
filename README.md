# NEURAL-STYLE-TRANSFER
Created a Neural Style Transfer model that blends artistic styles with real images using deep learning. Excited to explore creativity through AI-generated artwork.
company codtech it solutions

name tejas tagad

intern id CT04dr1129

Domian Artificial Intelligence

Duration 4 weeks

Mentor NEELA SANTOSH

##This project implements Neural Style Transfer (NST) using the VGG19 convolutional neural network in TensorFlow. Neural Style Transfer is a deep learning technique that synthesizes a new image by combining the content of one image with the style of another. It is a compelling application of convolutional neural networks, originally introduced by Gatys et al., which enables machines to "paint" new artworks by mimicking human-like creativity.

Objective The main objective of this project is to generate an image that preserves the content of a given input photograph (e.g., a photo of the Golden Gate Bridge) while adopting the artistic style of a second image (e.g., Van Gogh’s Starry Night). This is achieved by optimizing a loss function that balances content loss and style loss, computed using feature representations extracted from the VGG19 network.

Approach and Architecture The model used is the VGG19 neural network, a 19-layer deep CNN pre-trained on ImageNet. This network is known for its ability to extract rich hierarchical features from images, making it ideal for both content and style representation.

Content Image: Provides the structural elements or layout of the final output.

Style Image: Provides the artistic textures, brush strokes, and patterns.

VGG19 Feature Maps: Different layers capture different levels of abstraction; deeper layers capture content, while shallower layers capture textures and patterns.

Loss Function:

Content Loss: Calculated using activations from a deeper layer (e.g., block5_conv2), ensuring the generated image retains the primary objects and layout of the content image.

Style Loss: Calculated using the Gram Matrices from multiple shallow layers (e.g., block1_conv1 to block5_conv1), capturing correlations between feature maps to represent the overall style.

Total Loss: A weighted combination of content and style loss.

Training and Optimization An initial image (typically a copy of the content image) is iteratively updated using gradient descent to minimize the total loss. The optimization is performed using the Adam optimizer, and after each iteration, the image is clipped to keep pixel values within a valid range [0, 1].

Results The output is a stylized image that merges the visual aesthetics of the style image with the recognizable elements of the content image. In this notebook, the Golden Gate Bridge is rendered with the swirling, expressive brushwork of Starry Night, producing an impressive fusion of photography and classical art.

Applications Neural Style Transfer has broad applications in:

Digital Art and Design: Creating stylized portraits and artworks.

Augmented Reality (AR): Real-time video stylization.

Content Creation: Enhancing media in creative industries.

Conclusion This project showcases the intersection of deep learning and artistic expression. By leveraging the powerful feature representations of VGG19, it demonstrates how machines can produce creative outputs that emulate human art. The Google Colab implementation ensures accessibility, allowing users to experiment with their own content and style images with minimal setup.
