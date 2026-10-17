# Route 66 Dataset

A dataset for the food of the restaurant [Route 66](https://route66ourense.es/). The objective is to have multiple photos of every type of dish so later computer vision models can be used. Maybe image classification or generative models.

To add new photos, follow these rules:

1. Only one photo per dish. I don't want the same dish from multiple angles.

2. The photo should only have one dish in the frame and it should be properly cropped. The dish should be the main focus of the photo.

3. The dish should be photographed at the restaurant and complete (no bites taken).

4. A photo that has already been committed to the main branch shouldn't be modified in a new commit.

5. Each photo should be stored in the correct folder inside the [`data`](./data/). If the dish is a _Medio Bocata_, the folder is the normal name of the _Bocata_ plus `_H`. For example: [`data/Chevrolet_H`](./data/Chevrolet_H).

6. The name of the photo should be `YYYY-MM-DD_N`. `YYYY-MM-DD` is the date when the dish was eaten. `N` is a number that is used to differentiate between photos of the same type of dish taken on the same day. `N` should start at 1 and increase by 1 for each new photo of the same type of dish on the same day.
