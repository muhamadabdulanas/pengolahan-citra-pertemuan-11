# pengolahan-citra-pertemuan-11

#### Muhamad Abdul Anas
#### TI.22.A2

## Invert
#### import matplotlib.pyplot as plt
#### from skimage.morphology import convex_hull_image
#### from skimage import data, img_as_float
#### from skimage.util import invert

## Load the original image
#### image = invert(data.horse())

## Compute the convex hull of the image
#### chull = convex_hull_image(image)

## Plot the original and transformed images
#### fig, axes = plt.subplots(1, 2, figsize=(8, 4))
#### ax = axes.ravel()

#### ax[0].set_title('Original picture')
#### ax[0].imshow(image, cmap=plt.cm.gray)
####ax[0].set_axis_off()

#### ax[1].set_title('Transformed picture')
#### ax[1].imshow(chull, cmap=plt.cm.gray)
#### ax[1].set_axis_off()

#### plt.tight_layout()
#### plt.show()
