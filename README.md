# BYCT-Data-Science-Challenge-Week-2
Exploring Video Game Sales  

This challenge dives into the video game sales dataset, shifting the focus from data engineering to analysis and visualization. Utilizing libraries like pandas, matplotlib,plotly.express,scipy,KNNImputer,scikit-learn and seaborn to uncover insights from the data.

About the Dataset: Video Games Sales Dataset
- Dataset: Video Games Sales Dataset , size: 55,000 (as of April 2019) , source: Scraped from vgchartz.com
- Content: Game details: Name, Platform, Genre, ESRB Rating, Sales figures: Total Shipped copies, Global Sales (worldwide), Sales figures 
  for North America (NA_Sales), Europe (PAL_Sales), Japan (JP_Sales), and Other regions.
- Review scores: Critic Score (from 10), User Score (from 10)
- Release Year.
  
Problem Description:
As a data analyst for a gaming company that is preparing to launch a new video game, you are tasked to analyze a comprehensive dataset of video game sales to uncover these insights. By providing a detailed analysis and help the company make data-driven decisions on game development, marketing strategies, and sales forecasts.

Lets get started....................................

STEP1#: Here are general instructions on how to run scripts or notebooks:
Assuming you have the necessary software (Jupyter Notebook) and dependencies installed, 
- Choose a Text Editor or IDE e.g Python scripts can be edited in editors like VS Code, Sublime Text, or IDEs like PyCharm,Jupyter 
  Notebook.
- Install Jupyter Notebook using pip (Python's package installer) by running pip install notebook.
- Start Jupyter Notebook Server: Open a terminal or command prompt, navigate to the directory where you want to store your notebooks 
  (using cd), type jupyter notebook and press Enter.
  This will start the Jupyter Notebook server and open your default web browser to the Jupyter Dashboard.
- Create or Open a Notebook: In the Jupyter Dashboard, click on "New" and choose the appropriate kernel (e.g., Python 3) to create a new 
  notebook  OR navigate to an existing notebook file (.ipynb) and click to open it.
- Run Cells in the Notebook: Jupyter Notebooks are divided into cells. Each cell can contain code, markdown text, or raw text.
  To run a cell containing code, click on the cell and press Shift + Enter or use the "Run" button in the toolbar above the notebook.
- Interact with the Notebook: As you run cells, you'll see output directly below each code cell.
  Markdown cells render formatted text (like this list) when run. They are editable and re-run cells.
- Save and Close: Save your notebook periodically using Ctrl + S or by clicking the "Save" button.
  Close the notebook by closing the browser tab or stopping the Jupyter server in the terminal (Ctrl + C and confirm with y).
  
STEP2#:CODE - _Project Objectives carried out_

  Set 1: Data Cleaning and Exploration (Easy):
   - Imported the neccesarry librabies like pandas, matplotlib, plotly.express,scipy, KNNImputer,scikit-learn and seaborn, Load the video 
     game data using pandas.read_csv and Printed the first few rows of the data to get a sense of its structure.
      _VGS_data= pd.read_csv(r'C:/Users/Christiana/Desktop/BYCT-Data Science Challenge/vgsales-12-4-2019.csv')
      VGS_data(10)_
   - Data summary:Get basic information about the data using df.info(), Described the numerical columns using df.describe(), Identify and handle missing values 
     (e.g. dropping irrelevant rows, imputing missing values).
   - Visualize data distribution: Created histograms and density plots for key numerical columns like "Critic Score," "User Score," and "Global_Sales" using 
     matplotlib or seaborn.
     
  Set 2: Basic Grouping and Analysis (Medium):
   - Top Genres by Sales:Group the data by "Genre" using the df.groupby(), calculated the total global sales for each genre and plotted a bar chart (using 
     matplotlib or seaborn) to visualize the top-selling genres.
   - Correlation between Scores and Sales: Calculated the correlation coefficient between "Critic Score" and "Global_Sales" using pandas and discuss the 
     interpretation of the correlation value.
      _corr_coef = VGS_data[['Critic_Score','Global_Sales']].corr()
      corr_coef_
   - Sales Over Time: Grouped the data by "Year" and calculate the average "Global_Sales" for each year and plotted a line chart (using matplotlib or seaborn) 
     to visualize the trend of global sales over time.
     
  Set 3: Advanced Analysis and Visualization (Advanced)
   - Platform Comparison: Analyze the sales performance of a specific genre across different platforms (e.g., PS4, XOne) and plotted a boxplot (using seaborn) 
     to compare the distribution of "Global_Sales" for that genre across platforms.
   - Interactive Visualization (Bonus): Utilize libraries like Plotly or Bokeh to create interactive visualizations that allow users to explore the data 
     dynamically (e.g., filtering by genre, platform, or year).
     
 Set 4: Predicting Sales:
  -  Explored building a simple linear regression model (using libraries like scikit-learn) to predict "Global_Sales" based on "Critic Score" and "User Score".
  -  Lastly, evaluated the model's performance and visualized the results.

STEP3#: ASSUMPTIONS MADE
- Performance: Presumed reasonable data sizes for efficient processing and prediction (i.e making informed assumptions about that data volumes will be efficient to balance between operational efficiency and computational capability, ensuring that the system performs optimally under expected conditions). 
  
STEP4#: CHALLENGES ENCOUNTERED...sigh Hmmmmmmmmmmmmmmmmmmmmmmmm

Technical Challenges: These challenges were met in areas like:
   - Filling/Replacing missing values appropriately
   - Grouping :In set3, Platform Comparison
   - Optimizing database queries for large datasets required iterative improvements.
   - Visualizatation:In both, Visualizing boxplot for Platform Comparison and visualizing the prediction results.
     
Non-technical challenges:
   - Low power supply
   - Poor network stability for further research
   - Inadequate sleep

Learning Resources:

1. Youtube Chanels
- Numpy vs. Pandas: https://www.youtube.com/watch?v=KHoEbRH46Zk&pp=ygUTcGFuZGFzIGNyYXNoIGNvdXJzZQ%3D%3D

- Pandas Crash Course: https://www.youtube.com/watch?v=UB3DE5Bgfx4

- Pandas Cleaning: https://www.youtube.com/watch?v=bDhvCp3_lYw&pp=ygUbcGFuZGFzIGRhdGEgY2xlYW5pbmcgY291cnNl

- Another Data Cleaning (Real World): https://www.youtube.com/watch?v=iaZQF8SLHJs

- EDA with Pandas: https://www.youtube.com/watch?v=xi0vhXFPegw&pp=ygUacGFuZGFzICBkYXRhIHZpc3VhbGl6YXRpb24%3D

- Data Visualisation with Matplotlib: https://www.youtube.com/watch?v=a9UrKTVEeZA&pp=ygUacGFuZGFzICBkYXRhIHZpc3VhbGl6YXRpb24%3D

- Matplotlib: https://www.youtube.com/watch?v=0P7QnIQDBJY&pp=ygUlcGFuZGFzIGFuZCBtYXRwbG90IGRhdGEgdmlzdWFsaXphdGlvbg%3D%3D

- Seaborn: https://www.youtube.com/watch?v=ooqXQ37XHMM&pp=ygUac2VhYm9ybiBkYXRhIHZpc3VhbGl6YXRpb24%3D

- Handling Missing Data: https://www.youtube.com/watch?v=P_iMSYQnqac

- Handling Missing Data (2): https://www.youtube.com/watch?v=uDr67HBIPz8
2. W3 Schools, GeekforGeeks,Stackoverflow,
