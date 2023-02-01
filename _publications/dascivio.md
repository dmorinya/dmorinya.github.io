---
title: "Data science against gender-based violence"
permalink: /publications/
author_profile: true
---

Introduction
------
Gender-based violence is the violence suffered by women for the sole reason of being so and is the
most serious manifestation of patriarchal culture, taking women's lives or impeding the full
development of their rights, equal opportunities, and freedoms. In Spain, in the period 2010-2021, 653
women have lost their lives due to gender-based violence, and 7 in 2022 (until March 14th). According
to the Statistical Dossier of Gender-Based Violence 2020 published by the Catalan Women's Institute,
more than 16,000 complaints were lodged in Catalonia in 2019, 82% of which occurred in the scope of
a sentimental partnership. Figure 1 depicts the number of gender-based violence reported cases in the
different geographic areas of a particular health region in Catalonia, and it can be seen that the Covid-
19 pandemic has increased the number of reported cases dramatically, especially due to a differential
behavior during the pandemic (mobility restrictions, mandatory confinements), and a training
intervention conducted over health professionals in this area starting in mid 2018. Despite the large
number of complaints, it is suspected that they represent only a small portion of the cases occurring,
as for very different reasons, the victims often decide not to report the assaults they suffer.

![fig1](/images/fig1.png)
*Figure 1. Reported monthly cases of gender-based violence in each area of the North Metropolitan
Region in Catalonia (Spain).*

As reported in the document on tackling sexual violence in Catalonia, being a victim of sexual violence
is often fraught with guilt that can lead to denial of sexual violence. Therefore, it is reasonable to think
that the number of diagnoses related to gender-based violence recorded in the public health system
databases may be underestimating the magnitude of the problem. It is clear that once an estimate of
the real extent of the problem has been obtained, it would be very useful not to leave the decision to alert about a possible case of gender-based violence (especially for suspicious unconfirmed cases) to
health professionals but providing them with a tool that can do it automatically, based on artificial
intelligence methods and capable of identifying the clinical and sociodemographic characteristics that
modify the likelihood that a woman might be a victim of gender-based violence.
In 2019, the Ministry of Equity of the Spanish Government conducted a large survey on over 9,500
women over 16 years old focused on studying the prevalence of gender-based violence in Spain and
detecting potentially vulnerable subpopulations. As can be seen in Figure 2, the proportion of women
reporting to have suffered physical or sexual violence is not uniform across the Spanish provinces,
ranging from 7% to 45%. Also shocking is the result that, among these women, only a small fraction of
them have searched for health services (excluding hospitalization), and that there is a negative
correlation between the proportion of gender-based violence victims and usage of health services
(correlation of -0.26, 90% CI: -0.47 to -0.04), probably related to factors like rurality, ease of access to
health services and different age structures among provinces, which will also be accounted for in the
framework of this project.

![fig2](/images/fig2.png)
*Figure 2. Estimated proportion (in percentage) of gender-based violence (physical and/or sexual) in
each Spanish province (upper map) and estimated proportion (in percentage) of usage of health
services excluding hospitalization among gender-based violence victims (lower map). Source: Self-
generated based on data from the population-level survey on gender-based violence in Spain.*

Aims and hypotheses
------
This project's overarching objective is to improve the social and health care model for the victim and
her environment in cases of gender-based violence, using advanced data science and mathematical
modeling methods. We have set four specific objectives, which are further described below:

O1. Estimate the actual evolution of the number of gender-based violence cases, also covering the
unreported cases, using the time series of registered cases by basic health area corresponding to the
Northern Metropolitan Health Region.

O2. Quantify the impact in reducing the underreporting issue of the new protocol to prevent gender-
based violence introduced in the primary care system in the Northern Metropolitan Health Region in
Catalonia in June 2018 and the training intervention conducted to sensibilize involved health
professionals.

O3. Predict when women may be victims of gender-based violence early on by developing new
ensemble models based on a broad collection of clinical and sociodemographic features and identify
which of these features are best predictors of such violence to create new knowledge in the field.

O4. Develop technology capable of predicting women's characteristics compatible with a scenario of
gender-based violence to assist health and social care professionals in identifying potential scenarios
of this sort of violence in a clear and transparent manner.

Innovation
------
The current project is novel at least in two ways: First, it uses real-world data that have not been
analyzed in much detail before to estimate underreporting, predict potential victims of gender-based
violence as well as generate accurate knowledge in the field to allow professionals updating their
protocols and perspectives on certain aspects of the problem. Second, we will develop more flexible
and appropriate methods for underreporting estimation and predictive purposes (see specific
objectives described above), with the aim of improving the existing counterparts’ performances, thus
providing more accurate outcomes and outputs from this project.
In terms of data, for underreporting estimation (specific objectives O1. and O2., see above), we will
use all the primary care diagnoses related to gender-based violence reported in the Northern
Metropolitan Health Region in Catalonia (Spain) between January 1, 2010, and December 31, 2021. To
date, underreporting in such data has not been studied or accurately estimated, even though
professionals in the field are aware that this is a common phenomenon of gender-based violence data
which worsen inferences and related conclusions. In addition, for the predictive purposes outlined in
the third and fourth specific objectives (see specific objectives O3. and O4. above), we will use data
from the macro-survey on violence against women, which was performed on a representative sample
of 9.568 women aged over 16. The survey covered aspects related to sexual, psychological, and
economic violence from a current or former partners, physical and sexual violence from non-partners,
sexual harassment, and stalking (all these manifestations of violence englobed in the concept of
gender-based violence), as well as other demographical and societal data such as age, education level,
country of birth, marital status at the time of the survey, employment detail at the time of the survey,
number of sons, partner’s gender, partner’s education level and partner's nationality, among others.
For knowledge generation in the field (stated in the specific objective O3.), we will use data from the
macro-survey described above, e.g., detecting the variables that best predicted risk of suffering
gender-based violence, as well as new data consisting of women's characteristics such as age and
nationality, and women’s health indicators such as the number of medical visits, number and status of
pregnancies, number of miscarriages, urgency contraception usage, tobacco and alcohol status,
physical activity, sexual relations, STI risk status, number of cytologies. These characteristics will be
available for a sample of women who have already been diagnosed as victims of gender-based violence, as well as for a sample of women from the same region who have used the public health
system at least once during the same time period although they were not diagnosed as victims of
gender-based violence. We will use two different sets of data to create knowledge in the form of
features or attributes that best characterize victims of gender-based violence given that the macro-
survey does not contain information related to women’s health status, and this may be also relevant
for the quick identification of potential victims, especially for the health professionals. To our
knowledge, none of these datasets have been used for predictive purposes or for field knowledge
production (in the terms stated in this project, i.e., for the detection of features as good predictors of
gender-based violence) so far, even though both contain a wealth of rich and accurate information.
In terms of methods development, for the purpose of underreporting estimation, we will extend
recently proposed models based on longitudinal data analysis3,5 to analyze whether the incidence of
the reported cases of gender-based violence has been underreported, as well as to estimate the
frequency and intensity of the underreporting issue (specific objectives O1. and O2.). This model will
be extended in different ways: Firstly, we will consider a time-varying underreporting scenario, i.e., we
will allow underreporting parameters (frequency and intensity) to vary over time by considering
appropriate and flexible functions. Second, we will investigate more complex structures for the latent
processes, e.g., allowing more complex auto-correlation structures that may be more realistic, as well
as more flexible models for characterizing the underreporting phenomenon. In addition, we will
explore new alternatives for developing models for underreporting identification and estimation
following methods based on N-mixture models, Bayesian approaches or capture-recapture
methods, among other approaches.
Finally, for achieving the third and fourth specific objectives (O3. and O4.), we will develop: (i) methods
for variable selection and dimensionality reduction and (ii) prediction methods based on ensemble
approaches. For the first point before, given that a large number of important potential predictors for
gender-based violence identification is available, we will investigate and develop new methods for
variable selection based on knockoffs. Knockoff-based methods are a general framework for
controlling the false discovery rate in variable selection procedures. The idea here is to investigate
some of these existing techniques to select a collection of variables that are actually effective
predictors of gender-based violence and extend some of the existing knockoff-based methods to
improve the current project's outcomes. Techniques for variable selection based on knockoffs are
relatively new since they have not been explored in detail to date, and while there is a lot of good
literature out there, there is still a lot of room for improvements in this area. For the second point, using the outcomes provided by the previous step (i), we will develop new prediction models based on
ensemble techniques, which very often provide better predictive performances controlling
overfitting, lessening the curse of dimensionality, mitigating class imbalances, etc. The idea behind
ensemble techniques is to optimally combine a varied collection of weak learners that each captures
specific aspects of the data, and a key point is thus the way we combine such weak learners. This
project will build on different ensemble approaches, including adaptive boosting (AdaBoost),
gradient boosting machines, stacked generalization techniques, and ensemble deep learning. We will
extend some of these ensemble methods to provide a powerful predictive machine able to predict
women at risk of suffering gender-based violence, guaranteeing both low false-positive and false-
negative rates. To date, these approaches have never been used before to prevent gender-based
violence in the terms proposed by this project.

All data handling and statistical analyses will be conducted by developing new programs based on R
language (version 4.1.0), and all codes and algorithms generated by this project will be available from
public repositories as GitHub (https://github.com/) or CRAN (https://cran.r-project.org/) for full
transparency.

Further details related to methods development will be described below in Section *Methodology*.

Acknowledgements
------
This research has been funded by the Social Observatory of the "la Caixa" Foundation as part of
the project LCF/PR/SR22/52570005.

![logo](/images/logo.png)