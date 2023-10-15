# First, we need to connect to the terminal
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/ce743481-5f39-4cc0-9a58-19755c2ee941)

# Next, we install Git Bash, paste it into the terminal, and clone the repository
```
git clone https://github.com/git/git
```
Let's move on to installing SnarkOS

`sudo apt-get update`

`sudo apt-get upgrade`

Here we click `Y`

`sudo apt-get install`

`screen -S anasayfa`

Next, install Rust

`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/997fe54b-2e2b-4979-973f-fcd541bdc757)
*Next, clone the desired repository:**
`git clone https://github.com/AleoHQ/snarkOS.git --depth 1`
Next, go to the SnarkOS directory and install Cargo
`cd snarkOS`
`./build_ubuntu.sh`
After this command, the download will start, you need to wait for the process to complete, it takes 5-7 minutes
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/928f9106-3bc8-463a-9140-8bfd29d8fb7d)
`source $HOME/.cargo/env`
Install Cargo and wait for the installation to complete in a few minutes
`cargo install --path .`
Next, we will install and configure the Leo programming language
`cd`
`git clone https://github.com/AleoHQ/leo`
`cd leo`
`cargo install --path .`
After this command, the download will start again, and you will need to wait for it to complete.
`leo`
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/2d6896a1-51e2-4088-96d3-cdd3d879c0f5)
We are shown what commands we can use, let's continue with creating a new wallet or importing an existing one using the following commands:
`leo account new`
`leo account import YOUR_Private_Key`
Where instead of "YOUR_Private_Key" you need to insert your private wallet key, if you did everything correctly, you will get the following result:
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/82e1168d-ff32-4a11-b3b4-09028cded1d4)
Return to the terminal and enter `leo example`.
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/5e1a2d10-5dd2-4a71-8ae4-b7f45475e7fc)
We will be given the available options, let's try tictactoe:
`leo example tictactoe`
The result should be as follows:
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/1e475b61-dfcb-4880-9354-c370e2332fcd)
Next, for an illustrative example, let's run our program and see if it works, using the following command, enter the tictactoe directory:
`cd tictactoe`
And we do the launch as a team:
`leo run new`
If you have the same output from the terminal, I congratulate you, you have successfully deployed the application in Aleo
![image](https://github.com/AntonMatveychuk/Leo-Developer-Toolkit/assets/101927107/72bf6959-3160-4b14-bfb2-bdc2c1634268)






