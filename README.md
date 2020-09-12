# Deno Password Generator

this project aims to make it easy to generate strong passwords without the need to rely on third party tools or services that might use our passwords for malicious reasons. 
A password should only be known by its owner not another service or entity. Therefore it should be managed locally.
However generating secure passwords is pretty hard if not impossible. and as humans we surelly can't remember long randomly generated passwords.
But it does'nt have to be that hard. And thats what Deno Password Generator aims to solve.

## What you can do with it

- Generate very secure passwords from weak memorable passwords.
- Attach labels to passwords so that you know what they are used for and be able to generate them bac in case of loss
- Save the generated passwords locally so that you dont have to share them with 2nd or 3rd party entities

## How to use it

this script doesn't have a runnable file (.exe) yet but it will be coming soon.

- You need deno installed on your machine, atleast version 1.0.0
- You need some memorable password lets call it, **my_password**
- You need a label of the generated password lets call it, **my_label**
- You run the following command after **cloning the repository**.
  - `deno run main.ts --unstable --allow-read --allow-write --label my_label --pwd my_password`
  - You can make the password stronger by specifying a `--round <number>` where number is greater or equal than 1
  - To save the results to a file add this to the end of the first command `--save <path>` where path is where you want to store it.
- If you need help with how to use it run this command `deno run main.ts --unstable --allow-read --allow-write --help`