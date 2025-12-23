##READ ME
#How to activate pages:
1. Settings
2. Pages
3. Deploy from a branch -> main
4. Save

#Bonus
#How to utilize ssh key
1. Generate a new SSH key
	```bash 
	ssh-keygen -t ed25519 -C "seif.absalam@gmail.com"
	```
2. Start the SSH agent
	```bash
	eval "$(ssh-agent -s)"
	```
3. Add SSH key to the agent
	```bash
	ssh-add ~/.ssh/id_ed25519
	```
4. Copy the public key
5. Add SSH Key to GitHub
	a. settings
	b. SSH and GPG keys
	c. New SSH Key
	d. Key Type -> Authentication Key
	e. paste the SSH key copied earlier
	f. Add SSH Key
6. Test SSH Connection
	```bash
	ssh -T git@github.com
	```
	terminal asks for authentication then responds with
	```
	Hi seifabsalam! smth smth smth...
	```
