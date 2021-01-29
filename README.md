# Bank Accounts Manager 

## Description

Using OOP technique implement a back account management application providing followin functionalities:
- Add user; 
- Add account to user;
- Remove account;
- Add\substract money in\from an user account;
- Transfer money between two accounts (same user of different users);
- Display all accounts of a user;
- Display all accounts financial details: avarage account value, total value of all accounts of all users, user with maximum money in account;
- Interaction with system is done through a a text based (console) menu interface;

# Metrics Logger

## Description

- A "plug-in" Python mechanism that log metrics to persistent storage, be it a DB or file;
  - The sending should be abstract, nothing specific;
- This "plug-in" is used for functions. It gets the returned result and forwards it to the said persistent storage;
- This mechanism would be configurable, either through file, dictionary or Python object which would point to the said persistent storage and maybe format the metrics;
- This mechanism would not wait for confirmation from the storage space (optional);
- The metrics could be numeric results, events as string, timestamps or time intervals;

## Example

Considering an adding function (`def add(a: int, b: int) -> int`). If the "plug-in" mechanism is activated and it is configured to log messages in a file then for each method call a message in the following form will be displayed:

'12-02-2020 18:21 call func add (2, 10) -> 12' 
