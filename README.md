### Proportional Population Samples

  ```npm i sample-population```

Returns sample size for population numbers when supplied with the following paramaters

#### Example

```
var sample = require('sample-population');

var sampleSize = {
  population: 1234
};

var example = sample.population(sampleSize);

```
#### Parameters
```population: number```*required*

```confidence: number```*default* 1.98

The confidence level is the amount of uncertainty you can tolerate.
Default is set to 1.98 which is 95% confidence.

```errorMargin: number```*default* .5

The margin of error is the amount of error that you can tolerate. If 90% of respondents answer yes, while 10% answer no, you may be able to tolerate a larger amount of error than if the respondents are split 50-50 or 45-55.
Lower margin of error requires a larger sample size.
Default is set to .5

```response: number``` *default* .5

For each question, what do you expect the results will be? If the sample is skewed highly one way or the other,the population probably is, too. If you don't know, use 50%, which gives the largest sample size.
Default is set to .5
