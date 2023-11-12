# python_challenge
# Worked with classmate Dara Adesina on Module 3 project

# PyBank Explanation of code:
# Reading the CSV File:

# It uses the csv module to read data from the file named 'budget_data.csv'.
# The script creates a CSV reader and skips the header row using next(reader).
# Data Collection:

# Two lists, months and profit_losses, are initialized to collect the month and corresponding profit/loss data.
# Extracting Data:

# The script iterates through each row of the CSV file.
# It appends the month (row[0]) to the months list and the profit/loss value (int(row[1])) to the profit_losses list.
# Calculations:

# Total Months and Net Total: It counts the total number of months and calculates the net total amount of profit/losses using len() and sum() functions, respectively.

# Changes in Profit/Loss: It calculates the changes in profit/losses by iterating through the profit_losses list and storing the differences between consecutive months' values in the changes list.

# Average Change: It computes the average change in profit/loss by summing all changes and dividing by the count of changes.

# Greatest Increase and Decrease in Profits: It finds the greatest increase and decrease in profits by using the max() and min() functions on the changes list and retrieves the corresponding dates from the months list.

# Printing Results:

# The script prints the financial analysis results to the console, displaying:
# Total number of months
# Total amount of profit/loss
# Average change in profit/loss
# Greatest increase in profits and the corresponding date
# Greatest decrease in profits and the corresponding date

# PyPoll Explanation of code:
# Imports: It imports necessary modules - os and csv.

# File Initialization: It identifies the file name election_data.csv and initializes empty lists to store candidate names, their respective vote counts, and the percentage of votes they received.

# Variables Initialization: Sets total_votes to zero.

# Reading the CSV file:

# It opens the CSV file and reads its contents using the csv.reader.
# The header row is skipped (using next(csvreader)) as it's assumed to contain column names, not actual data.
# Vote Counting:

# It iterates through each row in the CSV.
# For each row:
# Increments the total_votes counter by 1.
# If the candidate's name (in the third column, row[2]) is not in the candidates list, it appends the name to the list and initializes their vote count to 1.
# If the candidate's name is already in the candidates list, it finds the index of the candidate and increments their vote count.
# Calculating Percentages:

# It calculates the percentage of votes each candidate received by dividing their vote count by the total_votes, rounding the percentage to the nearest whole number, formatting it as a string with three decimal places, and appending it to the percentage_votes list.
# Finding the Winner:

# It identifies the candidate with the maximum number of votes using max(number_votes) and captures their index. This determines the winner by finding the candidate at that index in the candidates list.
# Printing Results:

# It prints the election results to the console, displaying the total votes, individual candidate statistics (name, percentage of votes, and total votes received), and the name of the winning candidate.
# Writing to a File:

# It writes the same election results to a text file named output.txt line by line.
