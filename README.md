# Image_Based_Steganography_Using_Constrained_Least_Squares
This repository showcases a steganography technique embedding secret messages into images using constrained least squares. It covers encoding strategies, computational complexity, and practical implementations, ensuring hidden data transmission with minimal visible changes to the image.

## Overview
In this project, we delve into the fascinating realm of steganography, a technique used to
hide secret messages within an image. The objective is to embed the message in such a way that
the image appears unchanged to the naked eye, but a recipient with the right tools can decode
the hidden message. Our approach to steganography is based on the principle of constrained least
squares.

The secret message is represented as a Boolean vector, while the original image is represented as
an n-vector. The secret message is embedded into the image by adding a vector of modifications
to the original image vector. The modified image is then transmitted, and the recipient decodes
the message by multiplying the modified image by a specific matrix. The result is an estimate of
the original message.

Our focus will be on three key aspects:

1. **Encoding via least norm**: We will explore how to choose the modification vector to minimize
its norm, while ensuring that the decoded message is correct. We will provide a formula for
the modification vector in terms of the decoding matrix, a positive constant, and the original
image.

2. **Complexity**: We will analyze the computational complexity of encoding and decoding the
secret message. We will also estimate the time required for these operations on a computer
capable of carrying out 1 Gflop/s, considering a specific image size and message length.

3. **Practical Implementation**: We will demonstrate the application of this technique using an
actual image and a secret message. We will discuss how to choose the decoding matrix and
the positive constant to ensure that the original and modified images look the same, but the
secret message is still decoded correctly. We will also explore how to handle potential issues
such as values outside the acceptable range and round-off errors.

By the end of this project, we aim to provide a comprehensive understanding of this steganographic
technique and its practical implementation. We will also demonstrate how different secret messages
can be embedded in different original images, showcasing the versatility and potential applications
of this method.

### Additional Information

The repository also includes a `Report.pdf` that briefly explains our approach and methodology used to solve the problem.

