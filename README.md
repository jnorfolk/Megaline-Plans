# Megaline-Plans
Practicum Sprint 3 Project - Statistical Data Analysis

This was my third project during my Practicum data science program, where I analyzed a sample of Megaline phone plan users, subscribed to two plans. 
I evaluated the quality of the data, made corrections and created columns where necessary.
I used statistical testing to determine whether or not the two plans generate more revenue from a typical user, specifically a T-test and a Levene's test.

I felt like I established a solid basic foundation of applying statistics to data problems. Statistics is a topic that I now wish I had studied more in school, 
as I find its applications interesting. I will be studying more statistics on my own as I progress through my program.

## Data Format
The users table (data on users):
    user_id — unique user identifier
    first_name — user's name
    last_name — user's last name
    age — user's age (years)
    reg_date — subscription date (dd, mm, yy)
    churn_date — the date the user stopped using the service (if the value is missing, the calling plan was being used when this database was extracted)
    city — user's city of residence
    plan — calling plan name
The calls table (data on calls):
    id — unique call identifier
    call_date — call date
    duration — call duration (in minutes)
    user_id — the identifier of the user making the call
The messages table (data on texts):
    id — unique text message identifier
    message_date — text message date
    user_id — the identifier of the user sending the text
The internet table (data on web sessions):
    id — unique session identifier
    mb_used — the volume of data spent during the session (in megabytes)
    session_date — web session date
    user_id — user identifier
The plans table (data on the plans):
    plan_name — calling plan name
    usd_monthly_fee — monthly charge in US dollars
    minutes_included — monthly minute allowance
    messages_included — monthly text allowance
    mb_per_month_included — data volume allowance (in megabytes)
    usd_per_minute — price per minute after exceeding the package limits (e.g., if the package includes 100 minutes, the 101st minute will be charged)
    usd_per_message — price per text after exceeding the package limits
    usd_per_gb — price per extra gigabyte of data after exceeding the package limits (1 GB = 1024 megabytes)

## Data Usage
The data is provided by TripleTen and is proprietary, and therefore may not be published. It is, however, loaded into the notebook.
