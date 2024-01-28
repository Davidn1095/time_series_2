# time_series_2

# Reading CSV files
temp_test <- read.csv("DailyDelhiClimateTest.csv")
temp_train <- read.csv("DailyDelhiClimateTrain.csv")

# Combining data frames
temp_combined <- rbind(temp_test, temp_train)

# Creating a subset of the data
temp_combined_simple <- temp_combined[, c("date", "meantemp")][1:100, ]

# Displaying the first and last few rows
head(temp_combined_simple)
tail(temp_combined_simple)
