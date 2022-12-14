# Machine-Learning
Essay of machine learning application in supply chain
Data Science Application in Supply Chain 

Supply chain is about a network between companies and its supplier for production and distribute a product into end customer. This network includes some activities, people, entities, information, and sources. Supply chain is core in the production system, So it is a must to forecast the production need accurately. The accurate production forecast leads to minimizing cost. However, there is a gap between forecasting and the reality (Gunasekaran, 2004). Therefore, it is important to minimize the gap of forecasting in production with reality to minimize the cost.

Today’s information technology, have distrubted several business models. This disruption brings a whole list of opportunities and challenges for organizations and supply chain management domains (Aamer, 2018; Bower & Christensen, 1996; ER, 2019). One of the opportunities in supply chain domain is the increasing volume of data collection, referred to as big data. Big data is known as the five V’s: Volume, Velocity, Variety, Veracity, and Value (Affia et al., 2019; Jeble et al., 2018). Data analytics is needed to make big data have meaningful information, which plays an important role in supply chain management. Data analysis defined as the use of statistical and mathematical tools to analyze data and generate meaningful information for making decisions (Jeble et al., 2018). One of the technique of data analytics is machine learning that produce the prediction model automatically. Aamer et al (2021) said Machine learning algorithms can provide better accuracy and less computational cost for demand forecasting than traditional forecasting models. One of the trends in machine learning applications in demand forecasting. In this article, I will share about machine learning application for demand forecasting in pharmacy industry based on a journal from Zhu et al, 2021.

The pharmaceutical supply chain is a complex system in which drugs are delivered from the manufacturer to the patient through a distribution network. A simplified pharmacy distribution network highlighting what is pertinent to our work is depicted in Figure 1.

Figure 1 Illustration of a Pharma Distribution Network

The former usually have a large network, carry a wide variety of drugs, and distribute more frequently to hospitals, retail pharmacies, and home care providers, while the latter usually have a more controlled network, specialize in specialty drugs and distribute more frequently to offices. doctors, clinics, and independent specialty pharmacies (Xu et al. 2018). Regardless of the type, each trade partner (TP) has its own distribution network (DC), through which the points-of-care (POC) receives the drug.

Big data is obtained from our industry collaborators from the top two pharmaceutical manufacturers. The dataset consists of supply chain channel data on all pharmaceutical products owned by each manufacturer at the time of data collection. Each product is defined by a unique three-segment identifier, called an NDC. This is how the data collected from the business problem that need to solved.

The obtained data include all transaction (quality sold, TP, distributor, and DC's inventory level) between a drug manufacturer and TPs’ DCs are the needed data for forecast the demand. The data set was analyzed by descriptive statistics and also done with data cleaning. After that, the data was divided into learning and training data and also devided into three grouping schemes. The grouping schemesare by demand volume and volatility, by ATC code, and by clustering algorithm. This step makes the sample quality better.

With the groups obtained from the previous scheme, we further developed a learning model to predict future drug demand in each group. The model that usd is Machine learning algorithm. Since the data show a nonlinear pattern, we focus our discussion on the nonlinear method. In this reasearch, the author using recurrent neural networks to build the model because it is suitable for sequence data. 

After modeling, the step is evaluation. In this article, first step to evaluate their model is benchmarkingn with downstream distributors. Because the data is sequence, so there are lags in model result. So, to understand th emodel, we need decide suitable number of lags with parameter turning. For the final model evaluation is comparing the performance with normalized mean square error (NMSE), normalized mean absolute error (NMAE).

The result is RNN. So far, we have seen that RNN consistently outperforms other ML. RNNs are able to capture temporal features, for example, spikes in demand, due to their special design with memory cells that can recall the distant past. The result can be presented in meeting. 

Performance models in the pharma industry seems to have reached a bottleneck. At the same time, there are availability data and machine learning technologies. So, with that opportunity can help forecast the demand accurately. Accurate requests will keep costs to a minimum.


Referensi

Aamer, A. M. (2018). Outsourcing in non-developed supplier markets: a lean thinking approach. International Journal of Production Research, 56(18), 6048–6065. https://doi.org/10.1080/00207543.2018.1465609

Aamer, A., Eka Yani, L., & Alan Priyatna, I. (2020). Data analytics in the supply chain management: Review of machine learning applications in demand forecasting. Operations and Supply Chain Management: An International Journal, 14(1), 1-13.

Affia, I., Yani, L. P. E., & Aamer, A. M. (2019). Factors affecting IoT adoption in food supply chain management. 9th International Conference on Operations and Supply Chain Management, 19–24. 

Bower, JL, Christensen, C. (1996). Disruptive technologies: Catching the wave. Journal of Product Innovation Management, 13(1), 43–53. 

Gunasekaran, A., 2004. Supply chain management: Theory and applications. European Journal of Operational Research 159 (2), 265–268.

Jeble, S., Kumari, S., & Patil, Y. (2018). Role of big data in decision making. Operations and Supply Chain Management, 11(1), 36–44. https://doi.org/10.31387/oscm0300198

Zhu, X., Ninh, A., Zhao, H., & Liu, Z. (2021). Demand forecasting with supply‐chain information and machine learning: Evidence in the pharmaceutical industry. Production and Operations Management, 30(9), 3231-3252.

