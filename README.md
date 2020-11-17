# Bike_project
Explore data related to bike share systems of DIvvy Company for Chicago, New York City, and Washington to answer interesting questions about it by computing descriptive statistics.

EXPLORE US BIKESHARE DATA

Intro :

In this project, Python is used to explore data related to bike share systems for three major cities in the United States—Chicago, New York City, and Washington. You will write code to import the data and answer interesting questions about it by computing descriptive statistics. You will also write a script that takes in raw input to create an interactive experience in the terminal to present these statistics.

The Datasets of the cities consists of : 

Start Time (e.g., 2017-01-01 00:07:57)
End Time (e.g., 2017-01-01 00:20:53)
Trip Duration (in seconds - e.g., 776)
Start Station (e.g., Broadway & Barry Ave)
End Station (e.g., Sedgwick St & North Ave)
User Type (Subscriber or Customer)

The Chicago and New York City files also have the following two columns:

Gender
Birth Year

Code Structure : 

The code consists of 7 main functions 

1-getfilter():


    Asks user to specify a city, month, and day to analyze.

    Returns:
        (str) city - name of the city to analyze
        (str) month - name of the month to filter by, or 'all' to apply no month filter
        (str) day - name of the day of week to filter by, or 'all' to apply no day filter

2-load_data(city, month, day)

	 '''
    Loads data for the specified city and filters by month and day if applicable.

    Args:
        (str) city - name of the city to analyze
        (str) month - name of the month to filter by, or 'all' to apply no month filter
        (str) day - name of the day of week to filter by, or 'all' to apply no day filter
    Returns:
        df - Pandas DataFrame containing city data filtered by month and day
    '''
    
3-timestats(df)

   """
    Displays statistics on the most frequent times of travel as it calculates the most frequent month, day and hour of travel which depends on the user's filter.
    
    Args :
    df - Pandas DataFrame containing city data filtered by month, day, both, or none
    
    """

4- station_stats(df):
    
    """
    Displays statistics on the most popular start and end stations and trip from start to end.
    
    Args :
    df - Pandas DataFrame containing city data filtered by month, day, both, or none
    
    """
    
5- user_stats(df):

    """
    Displays statistics on bikeshare users like gender, birth date and user type  .
    
    Args :
    df - Pandas DataFrame containing city data filtered by month, day, both, or none
    """
    
6- trip_duration_stats(df):
    
    """
    Displays statistics on the total and average trip duration.
    
    Args :
    df - Pandas DataFrame containing city data filtered by month, day, both, or none
    """
    
7- display_user_data():
    """
    Displays data of five random users from the selected city and asking for input to display more random users.
    """
