# SMAIproject_TEAM21

## Performance-driven Batters’ Selection for Cricket Matches
by Aditi Bose, Saarthak Negi, Sriya Desabhatla

Dataset link: https://data.mendeley.com/datasets/fd23g625k7/1

Model weights link: https://drive.google.com/drive/folders/1yX-CDnBGOGgy6Te5arKm4r_4fLaB5llt?usp=drive_link 

1. train.ipynb
In the training phase, the dataset undergoes preprocessing including one-hot encoding for categorical variables. Multiple regression models, primarily ensemble-based, are trained with "runs" as the target variable. The weights for each model are saved individually. A generalized training function is also implemented to automate model selection by evaluating performance across models. Additionally, custom functions are defined to predict total runs scored by a team and identify the top four batters, based on input features: `player_country`, `opposition_country`, and `venue_type`.

2. eval.ipynb
This script loads all the saved model weights and evaluates each model using three performance metrics (e.g., MAE, RMSE, R²). It includes visual comparisons between predicted and actual runs to assess accuracy. Two comparative plots are generated to benchmark and contrast model performance, facilitating the selection of the most effective regression model.

3. inference (1).ipynb
In the inference module, saved models are used to test predictions for a fixed input scenario: India vs Australia under different venue types (home, away, neutral). For each venue, predicted team runs and top-performing batters are extracted. The results are visualized using comparative plots, emphasizing how predictions vary with venue type. These visualizations support the claim that `venue_type` significantly influences model output and plays a critical role in performance prediction—highlighting a novel aspect of the work.
