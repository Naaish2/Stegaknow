# Stegaknows

A steganography tool that conceals data within images. Supports both text-in-image and image-in-image embedding for secure data hiding.

## Features

• Hide text messages within images
• Embed images inside other images
• Secure data concealment using steganography techniques

## How It Works

Stegaknows uses the Least Significant Bit (LSB) substitution method for steganography. This technique embeds hidden data by modifying the least significant bits of the pixel values
in an image, making the changes imperceptible to the human eye.

### Text-in-Image Embedding

• Text data is converted to binary.
• The binary data is embedded into the LSBs of the image pixels.
• The modified image appears identical to the original but contains the hidden message.

### Image-in-Image Embedding

• The secondary image is compressed and converted to binary data.
• This binary data is embedded into the LSBs of the primary image pixels.
• The result is a single image containing the hidden image data.

This method ensures high security as the alterations are minimal and undetectable without the proper decoding algorithm.

## Tech Stack

• Frontend: Next.js, React, TypeScript
• Styling: Tailwind CSS, Radix UI
• Icons: Lucide React

## Installation

1. Clone the repository:
   git clone https://github.com/hamzahshahbazkhan/Stegaknows.git
   cd Stegaknows

2. Install dependencies:
   npm install

3. Run the development server:
   npm run dev

4. Open http://localhost:3000 http://localhost:3000 in your browser.

## Usage

• Upload an image to encode data.
• Enter text or select another image to hide.
• Download the encoded image.
• To decode, upload the encoded image and extract the hidden data.

## Build

To build the project for production:

npm run build
npm run start
