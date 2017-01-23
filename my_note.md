## Project: Build a Traffic Sign Recognition Program

(each try, ran at least three times)
### First Try: use the same settings as LeNet execise in the class 
(I ran several times and it goes from around 93% to 96%)
(it seems to bounce around the accurary in the end - epoch 8, 9, 10)

Accuracy: 96%. 

Training...

EPOCH 1 ...
Validation Accuracy = 0.670

EPOCH 2 ...
Validation Accuracy = 0.837

EPOCH 3 ...
Validation Accuracy = 0.888

EPOCH 4 ...
Validation Accuracy = 0.922

EPOCH 5 ...
Validation Accuracy = 0.935

EPOCH 6 ...
Validation Accuracy = 0.945

EPOCH 7 ...
Validation Accuracy = 0.947

EPOCH 8 ...
Validation Accuracy = 0.956

EPOCH 9 ...
Validation Accuracy = 0.961

EPOCH 10 ...
Validation Accuracy = 0.960

Model saved

### 1: change the learning rate to 0.0003 (from 0.001)
(accuracy went lower, but at least it won't bounce around.)
(try adding epoch)

Training...

EPOCH 1 ...
Validation Accuracy = 0.342

EPOCH 2 ...
Validation Accuracy = 0.567

EPOCH 3 ...
Validation Accuracy = 0.704

EPOCH 4 ...
Validation Accuracy = 0.772

EPOCH 5 ...
Validation Accuracy = 0.816

EPOCH 6 ...
Validation Accuracy = 0.848

EPOCH 7 ...
Validation Accuracy = 0.871

EPOCH 8 ...
Validation Accuracy = 0.891

EPOCH 9 ...
Validation Accuracy = 0.907

EPOCH 10 ...
Validation Accuracy = 0.918

Model savedTraining...

### 2: increase EPOCH to 20, keep learning rate to 0.0003
(increase the accuracy but the accuracy bounce around after 10 epoch).

EPOCH 1 ...
Validation Accuracy = 0.288

EPOCH 2 ...
Validation Accuracy = 0.504

EPOCH 3 ...
Validation Accuracy = 0.673

EPOCH 4 ...
Validation Accuracy = 0.771

EPOCH 5 ...
Validation Accuracy = 0.818

EPOCH 6 ...
Validation Accuracy = 0.842

EPOCH 7 ...
Validation Accuracy = 0.874

EPOCH 8 ...
Validation Accuracy = 0.892

EPOCH 9 ...
Validation Accuracy = 0.895

EPOCH 10 ...
Validation Accuracy = 0.910

EPOCH 11 ...
Validation Accuracy = 0.918

EPOCH 12 ...
Validation Accuracy = 0.912

EPOCH 13 ...
Validation Accuracy = 0.922

EPOCH 14 ...
Validation Accuracy = 0.934

EPOCH 15 ...
Validation Accuracy = 0.940

EPOCH 16 ...
Validation Accuracy = 0.933

EPOCH 17 ...
Validation Accuracy = 0.943

EPOCH 18 ...
Validation Accuracy = 0.945

EPOCH 19 ...
Validation Accuracy = 0.949

EPOCH 20 ...
Validation Accuracy = 0.951

Model saved


### 3: reduce the Batch Size to 64, increase EPOCH to 20, keep learning rate to 0.0003
(the accuracy started out better but didn't improve the final accuracyt too much, 
especially compare with original one)

Training...

EPOCH 1 ...
Validation Accuracy = 0.495

EPOCH 2 ...
Validation Accuracy = 0.754

EPOCH 3 ...
Validation Accuracy = 0.834

EPOCH 4 ...
Validation Accuracy = 0.876

EPOCH 5 ...
Validation Accuracy = 0.909

EPOCH 6 ...
Validation Accuracy = 0.910

EPOCH 7 ...
Validation Accuracy = 0.932

EPOCH 8 ...
Validation Accuracy = 0.929

EPOCH 9 ...
Validation Accuracy = 0.938

EPOCH 10 ...
Validation Accuracy = 0.945

EPOCH 11 ...
Validation Accuracy = 0.945

EPOCH 12 ...
Validation Accuracy = 0.954

EPOCH 13 ...
Validation Accuracy = 0.952

EPOCH 14 ...
Validation Accuracy = 0.946

EPOCH 15 ...
Validation Accuracy = 0.959

EPOCH 16 ...
Validation Accuracy = 0.953

EPOCH 17 ...
Validation Accuracy = 0.962

EPOCH 18 ...
Validation Accuracy = 0.965

EPOCH 19 ...
Validation Accuracy = 0.957

EPOCH 20 ...
Validation Accuracy = 0.957

Model saved

### 4: reduce the Batch Size to 64, increase EPOCH to 20, reduce learning to 0.0001
(accuracy doesn't improve.  Get really slow.  I think I can just use
the original settings for EPOCHS and learning rate, and reduce BATCH SIZE to 64
since BATCH SIZE seems to affect the accuracy for EPOCH 1.)
Training...

EPOCH 1 ...
Validation Accuracy = 0.290

EPOCH 2 ...
Validation Accuracy = 0.503

EPOCH 3 ...
Validation Accuracy = 0.655

EPOCH 4 ...
Validation Accuracy = 0.739

EPOCH 5 ...
Validation Accuracy = 0.783

EPOCH 6 ...
Validation Accuracy = 0.818

EPOCH 7 ...
Validation Accuracy = 0.839

EPOCH 8 ...
Validation Accuracy = 0.861

EPOCH 9 ...
Validation Accuracy = 0.869

EPOCH 10 ...
Validation Accuracy = 0.880

EPOCH 11 ...
Validation Accuracy = 0.893

EPOCH 12 ...
Validation Accuracy = 0.899

EPOCH 13 ...
Validation Accuracy = 0.910

EPOCH 14 ...
Validation Accuracy = 0.913

EPOCH 15 ...
Validation Accuracy = 0.913

EPOCH 16 ...
Validation Accuracy = 0.914

EPOCH 17 ...
Validation Accuracy = 0.923

EPOCH 18 ...
Validation Accuracy = 0.922

EPOCH 19 ...
Validation Accuracy = 0.928

EPOCH 20 ...
Validation Accuracy = 0.931

Model saved

### 5: reduce the Batch Size to 64 (EPOCH = 10, learning rate = 0.001)
Training...

EPOCH 1 ...
Validation Accuracy = 0.718

EPOCH 2 ...
Validation Accuracy = 0.847

EPOCH 3 ...
Validation Accuracy = 0.896

EPOCH 4 ...
Validation Accuracy = 0.892

EPOCH 5 ...
Validation Accuracy = 0.916

EPOCH 6 ...
Validation Accuracy = 0.932

EPOCH 7 ...
Validation Accuracy = 0.941

EPOCH 8 ...
Validation Accuracy = 0.946

EPOCH 9 ...
Validation Accuracy = 0.953

EPOCH 10 ...
Validation Accuracy = 0.938

Model saved

### 6: try filter size 3x3.  change convolution portion.  Batch Size still 64.
conv1 -> relu -> conv2 -> relu -> pool -> conv3 -> relu -> pool -> flattern -> FC -> FC -> FC

accuracy improves to 98.4%.  Not sure it is due to a filter size or extra conv layer.  
investigate to just add another layer next.  

Training...

EPOCH 1 ...
Validation Accuracy = 0.906

EPOCH 2 ...
Validation Accuracy = 0.957

EPOCH 3 ...
Validation Accuracy = 0.959

EPOCH 4 ...
Validation Accuracy = 0.969

EPOCH 5 ...
Validation Accuracy = 0.968

EPOCH 6 ...
Validation Accuracy = 0.979

EPOCH 7 ...
Validation Accuracy = 0.976

EPOCH 8 ...
Validation Accuracy = 0.979

EPOCH 9 ...
Validation Accuracy = 0.979

EPOCH 10 ...
Validation Accuracy = 0.984

Model saved

### 7: back to 5x5 filter but add one more conv layer.   Batch Size still 64.
conv1 -> relu -> conv2 -> relu -> pool -> conv3 -> relu -> pool -> flattern -> FC -> FC -> FC
(the extra conv doesn't seem to increase accuracy much.  3 x 3 filter seems to be a good idea
for this)

Training...

EPOCH 1 ...
Validation Accuracy = 0.792

EPOCH 2 ...
Validation Accuracy = 0.913

EPOCH 3 ...
Validation Accuracy = 0.936

EPOCH 4 ...
Validation Accuracy = 0.950

EPOCH 5 ...
Validation Accuracy = 0.958

EPOCH 6 ...
Validation Accuracy = 0.955

EPOCH 7 ...
Validation Accuracy = 0.966

EPOCH 8 ...
Validation Accuracy = 0.952

EPOCH 9 ...
Validation Accuracy = 0.971

EPOCH 10 ...
Validation Accuracy = 0.957

Model saved

### 8: Same as No.6.  Add more maps.
conv1 -> relu -> conv2 -> relu -> pool -> conv3 -> relu -> pool -> flattern -> FC -> FC -> FC
add extra maps to conv1, conv2, conv3.  
adding extra maps did not help much and made this very slow.  Going back to No. 6.

Training...

EPOCH 1 ...
Validation Accuracy = 0.860

EPOCH 2 ...
Validation Accuracy = 0.918

EPOCH 3 ...
Validation Accuracy = 0.957

EPOCH 4 ...
Validation Accuracy = 0.955

EPOCH 5 ...
Validation Accuracy = 0.968

EPOCH 6 ...
Validation Accuracy = 0.968

EPOCH 7 ...
Validation Accuracy = 0.974

EPOCH 8 ...
Validation Accuracy = 0.973

EPOCH 9 ...
Validation Accuracy = 0.973

EPOCH 10 ...
Validation Accuracy = 0.973

Model saved

### 9: Same as No.6.  Add another layer for FC.
thought about adding another layer for FC.  
conv1 -> relu -> conv2 -> relu -> pool -> conv3 -> relu -> pool -> flattern -> FC -> FC -> FC ->
(this started ok but then the accuracy goes up and down.  maybe try to set bigger learning rate?)

Training...

EPOCH 1 ...
Validation Accuracy = 0.853

EPOCH 2 ...
Validation Accuracy = 0.928

EPOCH 3 ...
Validation Accuracy = 0.951

EPOCH 4 ...
Validation Accuracy = 0.971

EPOCH 5 ...
Validation Accuracy = 0.957

EPOCH 6 ...
Validation Accuracy = 0.970

EPOCH 7 ...
Validation Accuracy = 0.976

EPOCH 8 ...
Validation Accuracy = 0.960

EPOCH 9 ...
Validation Accuracy = 0.940

EPOCH 10 ...
Validation Accuracy = 0.975

Model saved

### 10: Same as No.9.  (Add another layer for FC.)  Try a bigger learning rate
This still doesn't give me better accuracy. 

Training...

EPOCH 1 ...
Validation Accuracy = 0.880

EPOCH 2 ...
Validation Accuracy = 0.924

EPOCH 3 ...
Validation Accuracy = 0.947

EPOCH 4 ...
Validation Accuracy = 0.926

EPOCH 5 ...
Validation Accuracy = 0.955

EPOCH 6 ...
Validation Accuracy = 0.959

EPOCH 7 ...
Validation Accuracy = 0.971

EPOCH 8 ...
Validation Accuracy = 0.961

EPOCH 9 ...
Validation Accuracy = 0.953

EPOCH 10 ...
Validation Accuracy = 0.956

Model saved

### 11:  6: try filter size 3x3.  change convolution portion.  Batch Size still 64. Changed FC input/output number
(this reaches to 97.2% but the accuracy bounces up and down concerns me.)
Training...

EPOCH 1 ...
Validation Accuracy = 0.868

EPOCH 2 ...
Validation Accuracy = 0.935

EPOCH 3 ...
Validation Accuracy = 0.926

EPOCH 4 ...
Validation Accuracy = 0.953

EPOCH 5 ...
Validation Accuracy = 0.951

EPOCH 6 ...
Validation Accuracy = 0.966

EPOCH 7 ...
Validation Accuracy = 0.955

EPOCH 8 ...
Validation Accuracy = 0.969

EPOCH 9 ...
Validation Accuracy = 0.970

EPOCH 10 ...
Validation Accuracy = 0.972

Model saved
