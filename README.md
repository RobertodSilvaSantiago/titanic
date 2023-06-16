# titanic

This code is a command-line interface (CLI) program that provides various functionalities related to ship data. Here is an overview of what the code does:

It imports necessary libraries such as fuzzywuzzy for fuzzy string matching, matplotlib for data visualization, numpy for numerical operations, and folium for creating maps.
It imports a function called load_data from a module called load_data.
It defines some global variables such as ALL_DATA (loaded using the load_data function) which contains ship data, and BREAK_LOOP_SENTINEL which is a special value used to break the main loop.
It defines a set of required arguments and their format that can be used with certain commands.
The main function is the entry point of the program. It displays a starting message and enters a loop to continuously accept user input.
The execute_user_input function parses and executes user commands. It dispatches the command to the appropriate function based on the input.
There are several functions defined to handle specific commands:
get_all_countries_no_duplicates returns a list of unique country names.
get_top_countries returns a list of top countries based on the number of ships.
get_ships_by_types returns a list of ship types and their frequencies.
search_ship_fuzzy_partial searches for a partial match of ship names using fuzzy string matching and returns information about the matched ships.
create_speed_histogram generates a histogram of ship speeds using matplotlib.
save_map_with_ship_location creates a map using Folium library and saves it as an HTML file, showing the locations of ships.
exit_cmi returns a special value to exit the main loop.
The MENU_DISPATCH dictionary maps user commands to their respective functions.
The print_starting_message function displays a welcome message when the program starts.
The program calls the main function if it is run as a standalone script.
Overall, this code provides a command-line interface for interacting with ship data, allowing users to perform various operations such as retrieving country information, searching for ships, generating histograms, and creating maps.
