# Dreambooth Fine-tuning for Stable Diffusion using Diffusers

This repository demonstrates how to fine-tune Stable Diffusion using Dreambooth with the Hugging Face Diffusers library.

## Description

This project allows you to teach Stable Diffusion a new concept (a mini yellow alarm clock in this case) by fine-tuning the model on a small set of images. You can personalize the model to generate images of your own concepts.

## Key Features

- Fine-tunes the Stable Diffusion model using Dreambooth.
- Uses a small dataset of images to introduce a new concept.
- Provides options for prior preservation to maintain the class of the concept.
- Generates images based on various prompts.

## Requirements

- Python 3.8 or higher
- Other library requirements mentioned in the [requirements.txt](requirements.txt)

## Usage
It is recommended to directly run the python notebook on google colab as all the environment setup has been done according to that
1. **Prepare your dataset:**
    - Collect 3-5 images of the concept you want to introduce.
    - Save the images in a directory named `my_concept`.
2. **Configure settings:**
    - Set the `instance_prompt` to a descriptive prompt for your concept, including the initializer word (e.g., "a mini yellow alarm clock").
    - Enable or disable `prior_preservation` to control class preservation during training.
3. **Run the training process:**
    - Execute the code cells in the notebook to fine-tune the model.
4. **Generate images:**
    - Use the provided pipeline to generate images based on various prompts.
    - The generated images will be saved in the `stable_diffusion_outputs` directory.

## Example

The provided notebook demonstrates fine-tuning Stable Diffusion to recognize a "mini yellow alarm clock". You can adapt the code to train the model on your own concepts.

## Results

The fine-tuned model generates images that reflect the characteristics of the new concept when prompted accordingly. See the `stable_diffusion_outputs` directory for example images.

## License

This project is licensed under the MIT License.
