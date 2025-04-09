# WelcomeCode

#!/bin/bash

#Colours
greenColour="\e[0;32m\033[1m"
endColour="\033[0m\e[0m"
redColour="\e[0;31m\033[1m"
blueColour="\e[0;34m\033[1m"
yellowColour="\e[0;33m\033[1m"
purpleColour="\e[0;35m\033[1m"
turquoiseColour="\e[0;36m\033[1m"
grayColour="\e[0;37m\033[1m"

#Welcome Message
echo -e "\nWelcome $(whoami)"
echo -e "\n${yellowColour}[+]${endColour} Are you having a good day?"
echo -ne "\n(Yes/No): "
read Selection

#Message
function Message(){
if [[ "$Selection" == "Yes" || "$Selection" == "yes" ]]; then
        echo -e "\n${greenColour}That's Great To Hear!${endColour}"
elif [[ "$Selection" == "No" || "$Selection" == "no" ]]; then
        echo -e "\n${blueColour}Aww, I Hope Your Day Gets Better! T_T${endColour}"
else
        echo -e "\nInvalid Input"
fi
}

Message

