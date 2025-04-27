# stor390-homework-7-solved
**TO GET THIS SOLUTION VISIT:** [STOR390 HOMEWORK 7 Solved](https://www.ankitcodinghub.com/product/stor-390-homework-7-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;122168&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;STOR390 HOMEWORK 7 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Abstract: This homework explores the application of differential privacy via a biased randomized response mechanism, providing a generalized estimation formula for the proportion of sensitive observations. It also details the implementation of a K-Nearest Neighbors (KNN) classifier, demonstrating the creation and application of a Chebyshev distance function within the Iris dataset. Additionally, I explored the ethical challenges presented by the use of AI in healthcare, particularly focusing on the management of sensitive data in scenarios such as corporate acquisitions and access by insurance companies, highlighting the balance between technological benefits and privacy concerns and emphasizing the importance of ethical considerations in the deployment of AI technologies.

Question 1

Recall that in class we showed that for randomized response differential privacy based on a fair coin (that is a coin that lands heads up with probability 0.5), the estimatedproportionofincriminatingobservations𝑃̂ (inclass this was the estimated proportion of students having actually cheated) was given by 𝑃 = 2𝜋 −̂ where 𝜋 is the proportion of people answering affirmative to the incriminating question. I want you to generalize this result for a potentially biased coin. That is, for a differentially private mechanism that uses a coin landing heads up with probability 0 ≤ 𝜃 ≤ 1, find an estimate 𝑃̂ for the proportion of incriminating observations. This expression should be in terms of 𝜃 and 𝜋.

To generalize the result of the randomized response mechanism for a biased coin, we follow the methodology applied with a fair coin but adjust it to account for the bias in the coin flip probability.

Randomized Response Mechanism Setup:

1. Options for Each Respondent:

• Truthfully answer the question (e.g., such as having not cheated).

• Lie according to the outcome of a coin flip.

For a biased coin:

• Probability of flipping heads (𝜃) – the respondent lies.

• Probability of flipping tails (1 − 𝜃) – the respondent answers truthfully.

2. Ifthecoincomesupheads, therespondentanswers ”Yes” or ”No” irrespective of the truth and solely based on the result of the second coin flip.

3. If the coin comes up tails, the respondent answers truthfully.

Modeling Responses:

• Let 𝜋 be the proportion of people who answer ”Yes” to the question.

• When asked the question under this mechanism,

– The probability of a respondent saying ”Yes” because they are telling the truth (coin lands tails and they are in the truthful group): (1 −

𝜃)𝑃̂.

– The probability of a respondent saying ”Yes” because they are lying (coin lands heads twice): 𝜃2.

So, the total probability of receiving a ”Yes” response, denoted 𝑃̂, is given by the addition of the two outcomes: 𝜋 = 𝜃2 + (1 − 𝜃)𝑃̂

Solving for 𝜋:

We want to express 𝜋 in terms of 𝑃 and 𝜃. Rearranging the above equation:

𝜋 = 𝜃2 + (1 − 𝜃)𝑃̂ ⟹ 𝜋 − 𝜃2 = (1 − 𝜃)𝑃̂

⟹ 𝑃 =̂ 𝜋−𝜃1−𝜃2

Question 2

Next, show that this expression reduces to our result from class in the special case where 𝜃 = .

𝑃 =̂ 𝜋 − 𝜃 2 1 − 𝜃

Substituting 𝜃 with ,

𝜋 − ( 2

𝑃 =̂ 1 − (12)

Simplifying the numerator and denominator,

𝑃 =̂ 𝜋 −

Simplifying,

𝑃 = 2𝜋 −̂

This is the expression we derived in class for the estimated proportion of incriminating observations when using a fair coin for randomized response differential privacy.

Question 3

Consider the additive feature attribution model: 𝑔(𝑥′) =

𝜙0 + ∑𝑀𝑖=1 𝜙𝑖𝑥′𝑖 where we are aiming to explain prediction 𝑓 with model 𝑔 around input 𝑥 with simplified input 𝑥′. Moreover, 𝑀 is the number of input features.

Give an expression for the explanation model 𝑔 in the case where all attributes are meaningless, and interpret this expression. Secondly, give an expression for the relative contribution of feature 𝑖 to the explanation model.

Not covered so this was intentionally left blank.

Question 4

Part of having an explainable model is being able to implement the algorithm from scratch. Let’s try and do this with KNN. Write a function entitled 𝑐ℎ𝑒𝑏𝑦𝑐ℎ𝑒𝑣 that takes in two vectors and outputs the Chebychev or 𝐿∞ distance between said vectors. I will test your function on two vectors below. Then, write a 𝑛𝑒𝑎𝑟𝑒𝑠𝑡_𝑛𝑒𝑖𝑔ℎ𝑏𝑜𝑟𝑠 function that finds the user specified 𝑘 nearest neighbors according to a user specified distance function (in this case 𝐿∞) to a user specified data point observation.

Chebyshev distance: 6 KNN Data:

54 78 25

77 87 31

88 34 82

80 100 95

58 84 79

96 4 98

17 48 75

100 51 31

47 80 82

11 94 36

25 54 78

31 77 87

82 88 34

95 80 100

79 58 84

98 96 4

75 17 48

31 100 51

82 47 80

36 11 94

Test Point:

23 23 23

Nearest Neighbors:

17 48 75

75 17 48

54 78 25

Question 5

Finally create a knn_classifier function that takes the nearest neighbors specified from the above functions and assigns a class label based on the mode class label within these nearest neighbors. I will then test your functions by finding the five nearest neighbors to the very last observation in the 𝑖𝑟𝑖𝑠 dataset according to the 𝑐ℎ𝑒𝑏𝑦𝑐ℎ𝑒𝑣 distance and classifying this function accordingly.

Nearest Neighbors to the Observation:

6 5.4 3.9 1.7 0.4

5 5.0 3.6 1.4 0.2

6.1 5.4 3.9 1.7 0.4

5.1 5.0 3.6 1.4 0.2

6.2 5.4 3.9 1.7 0.4

Features of the Observation to be Classified:

Sepal.Length 5.9

Sepal.Width 3.0

Petal.Length 5.1

Petal.Width 1.8

Predicted Class of the Observation: setosa Actual Class of the Observation: virginica

Question 6

Interpret this output. Did you get the correct classification? Also, if you specified 𝐾 = 5, why do you have 7 observations included in the output dataframe?

The predicted class label by KNN was setosa, however, the true class was that of virginica. The code I wrote for KNN did not include what was written in class to include 7 observations, however, if I had written it in the same manner these additional outputs would have been the distances associated with the neighbor list.

Question 7

Earlier in this unit we learned about Google’s DeepMind assisting in the management of acute kidney injury. Assistance in the health care sector is always welcome, particularly if it benefits the well-being of the patient. Even so, algorithmic assistance necessitates the acquisition and retention of sensitive health care data. With this in mind, who should be privy to this sensitive information? In particular, is data transfer allowed if the company managing the software is subsumed? Should the data be made available to insurance companies who could use this to better calibrate their actuarial risk but also deny care? Stake a position and defend it using principles discussed from the class.

Sensitive health care data exists in a critical, complex intersection between technological innovation and personal privacy. The use of artificial intelligence, as exemplified by Google’s DeepMind in managing acute kidney injury, illustrates the potential of technology to enhance patient care. However, patient privacy is a cornerstone of the healthcare system, underpinning the principles of autonomy and consent. When patients share their information with healthcare providers, there is an implicit understanding that this exchange is for the sole purpose of enhancing their health and well-being. The moment this information becomes a commodity that can be transferred, especially withoutexplicitconsent, thisfoundationaltrustisviolated.

Inthe context of corporateacquisition, where the company responsible for managing healthcare software is absorbed by another entity, the continuity of data privacy policies becomes uncertain. It is imperative that patient data is not merely bundled into the assets transferred during such corporate movements. Instead, there must be a deliberate, transparent process that ensures patients are informed and their consent is obtained anew, thereby respecting their autonomy over personal information. When it comes to sharing patient data with insurance companies, the stakes are considerably higher. Insurance providers could argue that access to comprehensive data enables them to accurately calibrate actuarial risks. However, there is a thin line between informed risk calculation and the potential for discriminatory practices. If sensitive health data were freely available to these companies, it could lead to a situation where patients are penalized for conditions beyond their control, facing denial of coverage or prohibitive premiums. This not only challenges the ethical principle of justice, which advocates for fairness and equity, but also the principle of nonmaleficence, obliging us to refrain from causing harm to others. Furthermore, the governance of such data should be meticulously regulated to prevent misuse. Legislation akin to the Health Insurance Portability and Accountability Act (HIPAA) offers a framework that emphasizes patient rights and privacy. Strong regulatory oversight can ensure that insurance companies, should they be granted access, are not allowed to use this information to unjustly discriminate against individuals in need of coverage.

Inadvocatingforstringentprivacycontrolsandlimitedaccess to sensitive health care data, the principles of transparency and accountability cannot be overemphasized. Patients deserve clarity regarding the use of their data, with robust mechanisms in place to hold entities accountablefortheirdatapractices. Optingoutofdatasharingthat does not directly contribute to personal health care should always be an option available to patients.

Overall, while the integration of AI into healthcare is to be welcomed for its ability to enhance patient care, it must not be pursued at the expense of compromising patient privacy and the ethical standards that govern the healthcare profession. The priority must always be the rights and well-being of the individual patient, ensuring that advancementsintechnologyarematchedwithequallystrong protections for sensitive health information.
