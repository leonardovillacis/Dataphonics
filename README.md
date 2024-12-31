# Dataphonics
repositroy for python code that lets you listen to climate change data.

Want to listen to your time series data? Here's how.
Use the function SONIC with its many parameters to cater to you data structure.

SONIC(DF, TF, speed=0.4, reverse_data=True, invert_data=False, save_audio=True, save_plot=True, plot_filename='plot.png', audio_filename='output.wav', 
      xlabel="Years BP", ylabel="Values", title="Data Visualization", high_tone=650, low_tone=81.25, invert_yaxis=False, volume_factor=0.1)

DF is DataFrame object. Enter a list with the dataframe and all its variables, the age variable, and the climate variable you wish to plot.
    Example: DF = dfJouzel_ = [Jdata , Jdata.age_calBP , Jdata.Temperature]

TF is the TimeFrame object. Choose from the following list of time intervals with which data will be treated. Listen to your data at the rate you enter here.  
      minimum: minimum resolution of the record;
      fifty: 50 years;
      lifetime: 80 years;
      century: 100 years;
      country_time: 250 years;
      half_ocean_time: 500 years;
      ocean_time: 1000 years;
      greek_time: 3000 years;
      civilization_time: 6000 years;
      Holocene_time: 10,000 years;
      Homo_sapiens:300,000 years;
      Million: 1,000,000 years;
      Homo_time: 3,000,000 years;

speed is the time per sound or data point in seconds. Default is 0.4.

reverse_data allows to switch between listening from past to present or from present to past, according to data structure. Default is True.

invert_data assigns high and low pitch to lower or higher values. Default is False. i.e., Lower values are lower pitch. 

save_audio is the option to save audio. Default is True.

save_plot is the option to save the visualization. Default is True.

plot_filename allows you to set where and how you want to save the plot. 

audio_filename allows you to set where and how you want to save the audio.

xlabel sets x axis label. Default is "Years BP". 
 
ylabel sets y axis label. Default is "Values".
 
title set title for plot. Default is "Data Visualization".
 
high_tone assigns frequency of highest tone. Default is 650. 
 
low_tone assigns frequency of highest tone. Default is 81.25.
 
invert_yaxis allows y axis to be flipped. Default is False.
 
volume_factor sets volume. Default is 0.1.


Audio and plot will be saved to your computer. 

Example Function input:

SONIC(dfJouzel_,'civilization_time', plot_filename=r'D:\Jouzel.png',
     audio_filename=r'D:\Jouzel_audio.wav',
     ylabel='Temperature (°C)',title='EPICA Dome C Temperature')

See youtube channel for more examples!

https://www.youtube.com/@Dataphonics

Happy listening!




 
