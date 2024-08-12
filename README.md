# Building Trustworthy AI :bank:: <br>The Crucial Role of Explainabilty and Bias Elimination 
According to a recent PwC technology survey, 73%[^1] of US companies have integrated AI into some aspect of their operations, with this trend expected to accelerate. In the finance industry, AI tools are increasingly being used for critical functions such as fraud detection, customer personalization, risk management, and portfolio optimization, among others (refer to [figure 1](https://impact.economist.com/perspectives/sites/default/files/aiinfinancialservices.pdf)). 

CIBC, recognized for having Canada’s #1 rated mobile banking app, is making significant strides in this arena. Starting this August, CIBC announced a 12-month strategic collaboration with Creative Destruction Lab's **_Putting AI to Work Program_**[^2]. This partnership aims to enhance client services and improve operational efficiencies through AI-driven innovations. Additionally, Christina Kramer, CIBC's Head of Technology and Innovation, shared with [Bloomberg News](https://www.bloomberg.com/news/articles/2024-08-06/cibc-plans-hiring-spree-in-artificial-intelligence-data-jobs) that the bank plans to hire over 200 professionals in data and AI over the next year. This move underscores CIBC’s commitment to advancing its capabilities through pilot programs that leverage generative AI.

## AI Usage: Almost _TOO GOOD TO BE TRUE_, But Worth Careful Considerations
As you may notice now how important AI is for companies not only CIBC as its powerful usage, two potential factors behind should catch up attention when considering utilization of data to build powerful and trustworthy systems, further differentiating your AI from others. 

### 1. Making AI Explainable (XAI): Why Transparency Is Essential
> McKinsey has found that by incorprating explainability in algorithmic models, companies are more likely to row their yearly revenue 10% or more[^3].

> IBM shows users of its explainable AI platform realized a 15-30% improvement in model accuracy and $4.1-15.6 million more profit[^4].

The financial benefit shown above is quite straightforward to see why you want to have bring explainability for your models. But you may wonder why explainability can bring such huge impact, let's see what's going on behind the scene.

- **Unravel Black Box of Complex Machine Learning Models**:

In pratice, AI models trained input data and reached a particular decision, recommendation, or prediction through a black box where you cannot see what's going step by step explicitly. Explainability gives you the key to unlock the box to some extent and leads you towards a clear direction where you can improve, where you should fix, and how you can explain to non-technical audiences what's going on in a readable and clear manner.

- **Validation of Decision Making Through Human Engagement**:

After percieving the decomposition of complex ML models, you can validate if the result generated by models is trustworthy. For example, if a person who has zero income, lives in a low-income neightborhood, and low credit score is predicted by the model that he or she is qualified for loan, from a financial perception, you should not trust the result of the model, and there must be somthing going wrong. In this way, based on detected problems, tunning existing models will lead to higher model accuracy and performance.

- **Build Trust with Shareholders and Customers**:

If you cannot clearly explain why you come to the decisions using non-technical words towards shareholders and customers, instead throwing out something like "decsions are made by machines, let's just trust the AI", then arguments about fairness from customers and questions from shareholders lead to invevitable losses.

### Risks of Non-compliance:
- By-law, although there is no single global standard for AI transparency, there are some laws already exist, such as the General Data Protection Regulation (GDPR) in Europe, requiring copmanies explain to customers how AI made decisions on them; California Consumer Privacy Act (CCPA) also states customers have right to know inferences made about them by AI algorithms. Thus, non-copmlaince will lead to potential fines and litigation.
- Untrustworthy AI may also ffect reputation damage, loss of trust, and competitive disadvantage.

### Thoughts on Overcome the Issue:
Although it is tough to add explainability for models, there are several ways that increase explainability:
1. fit interpretable models like linear models and decision trees instead of complex ones like deep neural networking; the output coefficient values indicate clearly the effect of each component;
2. post-hoc explaination tools to see which feature is relatively more important, such as SHAP or LIME;
3. design tooling UI to explore model behaviours with different inputs as well as add dummy records to observe how the model responds.


### 2. Recognizing and Minimizing Data Bias: The Ethical Imperative


### Risks of Non-compliance:
- raise public concerns and arguments regarding fairness, ethics, and effectiveness;
- generate inaccurate, unreliable, and ineffective model predicitons;
- lead to legal and regulatory penalties;
- reputation damage, etc.

### Thoughts on Mitigate Bias:
Personally speaking, I don't believe all biases can be removed but minimized since defition of different biases is part subjective and part objective; there is no single version of definition of data bias. However, for sure, trying best to mitigate bias is always necessary:
1. most importantly, recognizing and admitting biases is always the first but hardest step; naturally, people are more likely to overlook and reluctant to admit it so that the outcome performance metrics look prettier and no complex further steps need to be taken;
2. evaluate codes or works by different team members to see if any individual bias may exist;
3. develop standardized guidlines on avoiding common biases;
4. develop fairness-aware machine learning models through pre-, in-, and post-processing techniques, e.g FaRM (Fairness-aware Recommendation with Meta-learning) reduces bias for sensitive features of users or items even in cold-start states for recommendation systems; adding fairness regularizers/constraints, etc.


## Conclusion
As AI-driven services are emerging everywhere nowadays, providing a trustworthy AI with high explainability and minimized bias would be the key to differentiate your AI from others thus increase your comptetitive advantage as well as to improve your model's performance, accuracy, and reliability. [CIBC's Trustworthy AI Commitment](https://www.cibc.com/content/dam/about_cibc/corporate_responsibility/pdfs/trustworthy-ai-guidelines-en.pdf) outlines its six trustworthy AI principles, indicating the importance of recognition and effort for using AI in banking industry. This is definitely a great example showing its copmetitive advantage from the aspects of social responsibility and transparency towards public.




[^1]: PwC's 2023 Emerging Technology Survey [https://www.pwc.com/us/en/tech-effect/emerging-tech/emtech-survey.html]
[^2]: CIBC forms strategic AI collaboration with Creative Destruction Lab [https://ca.finance.yahoo.com/news/cibc-forms-strategic-ai-collaboration-120000285.html?guccounter=1&guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAADzzlkAfFDiaYTQ9U_za2yXUr204ynHDx79DXhoSBZqiMLPvhQ-Fx_DsWJwrgtFDssT5YTQFR9XeP9E2kMnu30chqcW9rCO4W6jeOwyrskzcg4MGoLDOrLlI792h99xnPKRDJR0yWJ4LmZNM9OhYcZaXsxH-f1V6RiHKcwtUHe22
]
[^3]: Why businesses need explainable AI—and how to deliver it: [https://www.mckinsey.com/capabilities/quantumblack/our-insights/why-businesses-need-explainable-ai-and-how-to-deliver-it]
[^4]: What is explainable AI [https://www.ibm.com/topics/explainable-ai]

