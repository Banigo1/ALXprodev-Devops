# Advanced shell scripting

## Tasks

1. ### API Request Automation
mandatory
 
Objective: Automate the process of making API requests to the Pokémon API and saving the results to a file

Instructions:

Write a shell script that makes a request to the Pokémon API (https://pokeapi.co/api/v2/pokemon/ ) and retrieves data for a specific Pokémon Pikachu.

It should save the response to a json file: data.json

If the request fails, it should log the error to an error file: errors.txt

GitHub repository: ALXprodev-Devops
Directory: Advanced_shell
File: apiAutomation-0x00
  
1.  ### Extract Pokémon Data
mandatory
 
Objective: Use advanced text manipulation tools (jq, awk, sed) to extract specific data from the API response.

Instructions:

Write a script that extracts the Pokémon’s name, height, weight, and type from the JSON file created in Task 0.

Format the output in a human-readable way,“Pikachu is of type Electric, weighs 6kg, and is 0.4m tall.”

You should only use these commands: jq, awk, sed

GitHub repository: ALXprodev-Devops
Directory: Advanced_shell
File: data_extraction_automation-0x01
  
2.  ### Batch Pokémon Data Retrieval
mandatory
 
Objective: Automate the retrieval of data for multiple Pokémon and store it in separate files.

Instructions:

Create a script that loops through a list of Pokémon [Bulbasaur, Ivysaur, Venusaur, Charmander, Charmeleon.]

For each Pokémon, retrieve its data from the API and save it to a separate file named after the Pokémon (e.g., pikachu.json, bulbasaur.json…).

Handle any potential rate-limiting issues by adding a delay between requests.

GitHub repository: ALXprodev-Devops
Directory: Advanced_shell
File: batchProcessing-0x02
  
3.  ### Summarize Pokémon Data
mandatory
 
Objective: Create a report that summarizes data for multiple Pokémon.

Instructions:

Write a shell script that reads all the JSON files generated in Task 3 and extracts the name, height, and weight of each Pokémon.

Generate a CSV file containing the Pokémon’s name, height, and weight.

Use awk to calculate the average height and weight of all Pokémon in the report.

GitHub repository: ALXprodev-Devops
Directory: Advanced_shell
File: summaryData-0x03
  
4.  ### Error Handling and Retry Logic
mandatory
 
Objective: Add robust error handling and retry logic for API requests.

Instructions:

Modify the script from Task 2 to handle potential errors (e.g., network issues, invalid Pokémon names).

If an API request fails, implement a retry mechanism that attempts the request up to 3 times before logging the error and skipping to the next Pokémon.

GitHub repository: ALXprodev-Devops
Directory: Advanced_shell
File: batchProcessing-0x02
  
5.  ### Parallel Data Fetching
mandatory
 
Objective: Speed up data retrieval using parallel processing.

Instructions:

Write a script that fetches data for these Pokémon[ ] in parallel by leveraging background processes and process management tools.

Ensure that the script handles background processes properly and waits for all processes to complete before moving to the next step.

GitHub repository: ALXprodev-Devops
Directory: Advanced_shell
File: batchProcessing-0x04