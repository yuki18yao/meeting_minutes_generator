# meeting_minutes_generator
The application transcribes audio from a meeting, provides a summary of the discussion,  and extracts key points and action items.

## Warning
By default, the Whisper API only supports files that are less than 25 MB. If you have an audio file that is longer than that, you will need to break it up into chunks of 25 MB's or less or used a compressed audio format. To get the best performance, we suggest that you avoid breaking the audio up mid-sentence as this may cause some context to be lost.

Reffer to the following link: https://platform.openai.com/docs/guides/speech-to-text/longer-inputs 

## Example
Input: EarlingCall.mp3
Output: 
{
  'abstract_summary': "FinTech Plus had a strong Q2 in 2023, with a revenue of $125 million, a 25% increase YoY. The company's gross profit margin is at 58% due to cost efficiencies from its scalable business model. EBITDA surged to $37.5 million, with a 30% margin. Net income rose to $16 million from $10 million in Q2 2022. The company's total addressable market expanded with the introduction of new products. They diversified their asset-backed securities portfolio and invested in AAA-rated corporate bonds. The balance sheet shows total assets of $1.5 billion, liabilities of $900 million, and equity of $600 million. Customer acquisition costs dropped by 15%, and lifetime value grew by 25%. The company has a value-at-risk model and a healthy tier-one capital ratio of 12.5%. The forecast for the next quarter is positive, with expected revenue of $135 million and 8% QoQ growth. The upcoming IPO of their subsidiary, Pay Plus, is expected to raise $200 million.", 
  'key_points': '
    - FinTech Plus had a stellar Q2 with a revenue of $125 million, a 25% increase year over year.\n
    - Gross profit margin stands at 58% due to cost efficiencies gained from a scalable business model.\n
    - EBITDA surged to $37.5 million, translating to a remarkable 30% EBITDA margin.\n- Net income for the quarter rose to $16 million, a noteworthy increase from $10 million in Q2 2022.\n
    - Total addressable market has grown substantially due to the expansion of high-yield savings product line and the new RoboAdvisor platform.\n
    - Diversification of asset-backed securities portfolio, investing heavily in collateralized debt obligations and residential mortgage-backed securities.\n
    - Investment of $25 million in AAA-rated corporate bonds to enhance risk-adjusted returns.\n
    - Balance sheet shows total assets of $1.5 billion, total liabilities of $900 million, and equity base of $600 million.\n
    - Debt-to-equity ratio stands at 1.5, a healthy figure considering the expansionary phase.\n
    - Substantial organic user growth, with customer acquisition costs dropping by 15% and lifetime value growing by 25%.\n
    - LTVCAC ratio is at an impressive 3.5%.\n
    - Value-at-risk model in place for risk management, with a 99% confidence level indicating a maximum loss of $5 million in the next trading day.\n
    - Che next trading day.\n
    - Conservative approach to managing leverage, with a healthy tier-one capital ratio of 12.5%.\n
    - Positive forecast for the coming quarter, with expected revenue of around $135 million and 8% quarter-over-quarter growth.\n
    - Excitement about the upcoming IPO of fintech subsidiary, Pay Plus, expected to raise $200 million and bolster liquidity for aggressive growth strategies.', 
  'action_items': 'Based on the provided text, there are several action items mentioned:\n\n
  1. Continue diversifying the asset-backed securities portfolio by investing in collateralized debt obligations and residential mortgage-backed securities.\n
  2. Invest $25 million in AAA-rated corporate bonds to enhance risk-adjusted returns.\n
  3. Monitor the value-at-risk model to ensure that the maximum loss does not exceed $5 million in the next trading day.\n
  4. Prepare for the upcoming IPO of the fintech subsidiary, Pay Plus, to raise $200 million.\n
  5. Implement aggressive growth strategies after the IPO to take advantage of the increased liquidity.\n\n
  Please note that these action items are inferred from the information provided and may not capture all potential tasks or assignments.'}