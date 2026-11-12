# Sports Player Action Anticipation

## Project Overview
A deep learning project that uses sports video frames to recognize sports actions using CNN, GRU, LSTM, and pretrained ResNet18 models.

## Technologies Used
- Python
- PyTorch
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Google Colab

## Dataset
UCF101 dataset – six selected sports action categories:
- Basketball
- BasketballDunk
- Biking
- SoccerJuggling
- TennisSwing
- VolleyballSpiking

Total videos: 828

## Models Implemented
1. Custom CNN
2. CNN + GRU
3. CNN + LSTM
4. Pretrained ResNet18

## Results

| Model | Test Accuracy |
|---|---:|
| Custom CNN | 31.2% |
| GRU | 31.2% |
| LSTM | 28.8% |
| ResNet18 | 80.0% |

Best tuning configuration:
- Learning rate: 0.001
- Batch size: 16
- Validation accuracy: 34.68%
- Test accuracy: 32.8%

## Optimizer Comparison
Adam performed better than SGD in the experiment.

## Project Notebook
See `Sports_Player_Action_Anticipation.ipynb` for the implementation and experimental results.

## Limitation
UCF101 provides video-level action labels rather than timestamped match events. Therefore, this implementation is an action-recognition adaptation and not a complete next-event anticipation system.

## Future Improvements
- Use timestamped sports event datasets.
- Improve temporal action prediction.
- Explore attention mechanisms and transformer models.
