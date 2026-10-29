During my machine learning internship at Intelinair, I worked extensively with meteorological data retrieved through the IBM PAIRS weather API to develop weather-based crop disease-risk models. One particularly challenging variable was leaf-wetness duration (LWD), which estimates how long moisture remains on a plant's leaf surface.

The most confounding source of error was the difference between atmospheric measurements and actual leaf-surface conditions. Temperature, relative humidity, dewpoint, wind speed, and precipitation provide valuable information, but they do not directly indicate whether a leaf is wet. For example, high relative humidity does not necessarily mean condensation has occurred, while localized dew formation can occur without measurable rainfall.

I developed Python workflows to retrieve and process weather observations from IBM PAIRS and estimate LWD using meteorological variables and physically motivated relationships. A key consideration was distinguishing directly reported weather variables from derived estimates and understanding how uncertainty in the underlying observations could propagate into disease-risk predictions.

This experience taught me that data availability and numerical consistency do not guarantee physical accuracy. Even small systematic biases in environmental measurements can influence downstream decisions, particularly when models rely on thresholds.

Working with IBM weather data reinforced the importance of understanding measurement limitations, questioning assumptions, and treating derived environmental variables with appropriate uncertainty rather than accepting every API value as ground truth.
