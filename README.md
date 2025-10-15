Plan and Logic
Input: Get the path to the carrier image (e.g., input.png) and the secret text message.

Image Loading: Load the carrier image using Pillow.

Message Preparation:

Convert the text message into its binary representation.

Append a special "delimiter" (e.g., 0000000000000000 or a unique string of bits) to the binary message. This will signal the end of the message during extraction.

Pixel Iteration: Iterate through the pixels of the image, accessing their R, G, B values.

LSB Modification: For each color component (R, G, B) of each pixel:

Take the next bit from the prepared binary message.

Modify the LSB of the color component to match this message bit.

Crucially: Convert the pixel data back to a tuple (R, G, B) and update the image.

Saving: Save the modified image as a new file (e.g., stego_image.png).
