
<!-- README.md is generated from README.Rmd. Please edit that file -->

# statcanR

<!-- badges: start -->

[![Travis build
status](https://travis-ci.org/warint/statcanR.svg?branch=master)](https://travis-ci.org/warint/statcanR)
[![AppVeyor build
status](https://ci.appveyor.com/api/projects/status/github/warint/statcanR?branch=master&svg=true)](https://ci.appveyor.com/project/warint/statcanR)
<!-- badges: end -->

Allows an easy connection with R to Statistics Canada’s Web Data
Service. Open economic data (formerly known as CANSIM tables, now
identified by Product IDs (PID)) are accessible as a data frame,
directly in the user’s R environment.

## Installation

The released version of statcanR package is accessible through devtools.

``` r
install.packages("devtools")
devtools::install_github('warint/statcanR')
```

## Example

This section presents an example of how to use the statcanR R package
and its function sqs\_statcan\_data().

The following example is provided to illustrate how to use the function.
It consists in collecting some descriptive statistics about the Canadian
Labour Force at the federal, provincial and industrial levels, on a
monthly basis.

With a simple web search ‘statistics canada wages by industry
metropolitan area monthly’, the table number can easily be found on
Statisitcs Canada’s webpage. Here is below a figure that illustrates
this example, such as ‘14-10-0063-01’ for the Employee wages by
industry, monthly, unadjusted for seasonality at the ferederal and
provincial levels.

Once the table number is identified, the sqs\_statcan\_data() function
is easy to use in order to collect the data, as following:

``` r
library(statcanR)
mydata <- sqs_statcan_data("14-10-0063-01","eng")
```

### Why SQS?

SQS stands for SKEMA Quantum Studio, a research and technological
development centre based in Montreal, Canada, that serves as the engine
room for the SKEMA Global lab in AI.

SKEMA Quantum Studio is also a state-of-the-art platform developed by
our team that enables scholars, students and professors to access one of
the most powerful analytical tools in higher education. By using data
science and artificial intelligence within the platform, new theories,
methods and concepts are being developed to study globalisation,
innovation and digital transformations that our society faces.

To learn more about the SKEMA Quantum Studio and the mission of the
SKEMA Global Lab in AI, please visit the following websites :
[SQS](https://quantumstudio.skemagloballab.io) ; [Global
Lab](https://skemagloballab.io/).
