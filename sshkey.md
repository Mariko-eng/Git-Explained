You must generate a new SSH key to use for authentication. 

If you're unsure whether you already have an SSH key, you can check for existing keys.

Use The command to genearate ssh key for the main used for your Github account
# ssh-keygen -t ed25519 -C "your_email@example.com"

This creates a new SSH key, using the provided email as a label.

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location

Enter a file in which to save the key (/Users/user/.ssh/id_algorithm): [Press enter]

Enter ls | grep filename - to view the keys Eg 'ls | grep testKey'

Result is: 

1) testKey

2) testkey.pub

Two keys are then generated
1) One is private
2) Other is public

(You can copy the public key to the github, in setting/ssk keys) like so,

pbcopy < testKey.pub

Adding SSH Key to the ssh-agent
- modify the file '~/.ssh/config', As the link shown Below

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

