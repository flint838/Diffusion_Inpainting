# Diffusion_Inpainting
Image inpainting using Kandinsky 2.2 model. Uses prompts to fill in the missing sections
The Masker file masks the damaged parts of the image by adjusting the threshold values
The Kandinsky_2-2_dec file then uses prompts to fill in the missing regions with appropriate predicted pixels

![Screenshot from 2024-06-10 18-50-36 (2)](https://github.com/flint838/Diffusion_Inpainting/assets/80789060/72bd1a40-b711-4cc0-b6ed-9e4334b8080f)

This is the original damaged Image

The Masker applies the mask on the mssing areas with the adjusted threshold values of 200,255, like so:

_, damaged_mask = cv2.threshold(gray_painting, 200, 255, cv2.THRESH_BINARY)

This is present in the Masker.ipynb

![Screenshot from 2024-06-10 18-50-36 (3)](https://github.com/flint838/Diffusion_Inpainting/assets/80789060/deb4b295-fd2a-42b8-b1fb-0aa9e12ef190)

Masked Image

![Screenshot from 2024-06-10 18-50-36 (1) (1)](https://github.com/flint838/Diffusion_Inpainting/assets/80789060/8873b9dc-fd7d-455f-9c0e-810e437f373b)


Result
