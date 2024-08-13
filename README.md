# Building Trustworthy AI :bank:: <br>The Crucial Role of Explainabilty and Data Bias Elimination 
According to a recent PwC technology survey, 73%[^1] of US companies have integrated AI into some aspect of their operations, with this trend expected to accelerate. In the finance industry, AI tools are increasingly being used for critical functions such as fraud detection, customer personalization, risk management, and portfolio optimization, among others (refer to [figure 1](https://impact.economist.com/perspectives/sites/default/files/aiinfinancialservices.pdf)). 

CIBC, recognized for having Canada’s #1 rated mobile banking app, is making significant strides in this arena. Starting this August, CIBC announced a 12-month strategic collaboration with Creative Destruction Lab's **_Putting AI to Work Program_**[^2]. This partnership aims to enhance client services and improve operational efficiencies through AI-driven innovations. Additionally, Christina Kramer, CIBC's Head of Technology and Innovation, shared with [Bloomberg News](https://www.bloomberg.com/news/articles/2024-08-06/cibc-plans-hiring-spree-in-artificial-intelligence-data-jobs) that the bank plans to hire over 200 professionals in data and AI over the next year. This move underscores CIBC’s commitment to advancing its capabilities through pilot programs that leverage generative AI.

## AI Usage: Almost _TOO GOOD TO BE TRUE_, But Worth Careful Considerations
As AI continues to revolutionize industries, including at CIBC, its powerful potential is undeniable. However, to truly differentiate CIBC's AI from others, two critical factors must be prioritized when leveraging data to build powerful and trustworthy systems: **_explainability_** and **_robust data bias mitigation_**. By focusing on these, CIBC can not only enhance the performance of its AI models but also ensure that the systems align with the bank’s commitment to fairness, transparency, and client trust, further solidifying its leadership in the financial sector through AI-driven innovation.

### 1. Making AI Explainable (XAI): Why Transparency Is Essential
> McKinsey has found that by incorprating explainability in algorithmic models, companies are more likely to row their yearly revenue 10% or more[^3].

> IBM shows users of its explainable AI platform realized a 15-30% improvement in model accuracy and $4.1-15.6 million more profit[^4].

The financial benefits highlighted above make it clear why incorporating explainability into your models is essential. But you might be wondering why explainability has such a significant impact. Let’s explore what’s happening behind the scenes.

- **Unraveling Black Box of Complex Machine Learning Models**: <br>In pratice, AI models often operate as black boxes, where decisions, recommendations, or predictions are made without a clear view of the step-by-step process. Explainability provides the key to unlocking this black box, offering insights into where improvements can be made, where issues need to be fixed, and how to communicate the model’s processes to non-technical audiences in a clear and understandable way.

- **Validating of Decision Making Through Human Oversight**: <br>By understanding the inner workings of complex ML models, you can assess whether the outcomes they produce are reliable. For example, if a model predicts that a person with zero income, living in a low-income neighborhood, and with a low credit score qualifies for a loan, this raises red flags from a financial standpoint. Such scenarios indicate that something may be wrong with the model, prompting necessary adjustments. Addressing these issues through human oversight leads to higher accuracy and improved performance.

- **Building Trust with Shareholders and Customers**: <br>Being able to clearly explain how decisions are made, using straightforward language, is crucial for building trust with stakeholders and customers. If you simply defer to the notion that "decisions are made by machines" without offering clear explanations, you risk eroding confidence, raising concerns about fairness, and facing questions that can lead to significant losses. Transparent communication fosters trust and strengthens relationships with both shareholders and customers.

### Risks of Non-compliance:
- **Legal Repercussions**: While there isn’t a single global standard for AI transparency, regulations like the General Data Protection Regulation (GDPR) in Europe and the California Consumer Privacy Act (CCPA) are already in place. These laws require companies to explain how AI makes decisions about customers, and failure to comply can result in significant fines and legal actions.
- **Reputation and Trust**: An AI system perceived as untrustworthy can lead to severe reputational damage, loss of customer trust, and a competitive disadvantage. Companies that cannot clearly explain their AI’s decisions may find it increasingly difficult to maintain stakeholder confidence and market position.

### Thoughts on Overcome the Issue:
Enhancing model explainability can be challenging, but there are effective strategies to achieve it:
1. **Use Interpretable Models**: Opt for interpretable models like linear regression or decision trees over complex models like deep neural networks. These simpler models provide clear insights, with output coefficients directly indicating the impact of each feature.
2. **Apply Post-Hoc Explanation Tools**: Utilize tools like SHAP or LIME to analyze the relative importance of features, offering insights into how different factors influence the model’s decisions after the model has been trained.
3. **Develop Interactive Tooling**: Create user interfaces that allow for exploration of model behaviors with varying inputs. Additionally, introduce dummy records to observe how the model reacts, helping to identify areas for improvement and increase transparency.


### 2. Recognizing and Minimizing Data Bias: The Ethical Imperative
ALthough sample selection bias and inductive bias are also important to be mitigated, personally speaking, elimination of data bias, which is implicitly shown and is hard to be detected, is relatively more challenging

### Risks of Non-compliance:
- raise public concerns and arguments regarding fairness, ethics, and effectiveness;
- generate inaccurate, unreliable, and ineffective model predicitons;
- lead to legal and regulatory penalties;
- reputation damage, etc.

### Thoughts on Mitigate Data Bias:
Personally speaking, I don't believe all biases can be removed but minimized since defition of different biases is part subjective and part objective; there is no single version of definition of data bias. However, for sure, trying best to mitigate bias is always necessary:
1. most importantly, recognizing and admitting biases is always the first but hardest step; naturally, people are more likely to overlook and reluctant to admit it so that the outcome performance metrics look prettier and no complex further steps need to be taken;
2. evaluate codes or works by different team members to see if any individual bias may exist;
3. develop standardized guidlines on avoiding common biases;
4. develop fairness-aware machine learning models through pre-, in-, and post-processing techniques using packages like AI Fariness 360, fairlearn, etc.


## Conclusion
Documenting and clearly demonstrating to the public that your AI is transparent and trustworthy are also essential and beneficial. A great example is [CIBC's Trustworthy AI Commitment](https://www.cibc.com/content/dam/about_cibc/corporate_responsibility/pdfs/trustworthy-ai-guidelines-en.pdf), which outlines its six key principles that emphasize the bank's dedication to using AI responsibly in the banking industry. This commitment not only strengthens CIBC’s competitive edge but also demonstrates its leadership in social responsibility and transparency.



[^1]: PwC's 2023 Emerging Technology Survey [https://www.pwc.com/us/en/tech-effect/emerging-tech/emtech-survey.html]
[^2]: CIBC forms strategic AI collaboration with Creative Destruction Lab [https://ca.finance.yahoo.com/news/cibc-forms-strategic-ai-collaboration-120000285.html?guccounter=1&guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAADzzlkAfFDiaYTQ9U_za2yXUr204ynHDx79DXhoSBZqiMLPvhQ-Fx_DsWJwrgtFDssT5YTQFR9XeP9E2kMnu30chqcW9rCO4W6jeOwyrskzcg4MGoLDOrLlI792h99xnPKRDJR0yWJ4LmZNM9OhYcZaXsxH-f1V6RiHKcwtUHe22
]
[^3]: Why businesses need explainable AI—and how to deliver it: [https://www.mckinsey.com/capabilities/quantumblack/our-insights/why-businesses-need-explainable-ai-and-how-to-deliver-it]
[^4]: What is explainable AI [https://www.ibm.com/topics/explainable-ai]

