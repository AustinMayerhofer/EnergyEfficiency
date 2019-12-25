# Feature selection
## Forward selection
- Choosing "best" variable by testing its accuracy when added to the model's features.
- For the first round, X5 was the most accurate with an accuracy just below 80.
- For the second round, adding X7 was consistently the best as it yielded roughly a 86.3% accuracy rate every time.
- For the third round, X1, X2, and X3 all yielded similar results when added.
    - X5/X7/X1: roughly 91% with X4
    - X5/X7/X2: not quite as high as the X5/X7/X1/X4 model above.
    - X5/X7/X3: roughly 91% with X1.
    - X3 seemed to consistently have the best accuracy with X5 and X7 so choose that variable.
- Add X1, X2, getting best results so far. All combinations above 91%.
- Conclusion: Keep all variables because having X{1-8} gives a solid 91% accuracy without much performance dropoff.
- Take a look at variance next in variables.
## Backward selection
- For forward selection, X6 and X8 had negative accuracies so try removing them.
- all variables yielded 91.3%
- no X6/X8 yielded 91.2% and 91.3% (tad below all variables)
- no X6 went all the way down to 91.2% at times, 91.3% a lot and well above it. Seemed boom/bust compared to all variables.
- no X8 yielded consistently in the 91.1% and 91.2% so it was the worst performing.
- Conclusion: very minor difference between all variables and removing X6. Just keep all variables.