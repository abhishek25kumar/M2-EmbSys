# Complex Embedded System Case Study - Automated Teller Machine

## An ATM machine from an embedded systems point of view has:
 1. LCD or CRT screen to displays messages
 2. keypad for numeric input
 3. Cash dispenser
 4. Deposit slot
 5. Card reader
 6. Host Processor
 7. Receipt Printer

## Major Components Of ATM

1. **LCD or CRT Screen** :
The display screen displays the transaction information. Each step of withdrawal is shown by the display screen. A CRT screen or LCD screen is used by most of the ATMs.

2. **Keypad** : The card is recognized after the machine asks for further details like your identification number, withdrawal, and your balance inquiry Each card has a unique PIN so that there is little chance for some else to withdraw money from your account. There are separate laws to protect the PIN code while sending it to the host processor. The PIN is mostly sent in encrypted form. The keyboard contains 48 keys and is interfaced to the processor.

3. **Cash Dispenser** : The cash dispenser is the heart of the ATM. This is a central system of the ATM from where the required money is obtained. From this portion, the user can collect the money. The cash dispenser must count each bill and give the required amount. If in some cases the money is folded, it will be moved to another section and becomes the reject bit. All these actions are carried out by high precision sensors. A complete record of each transaction is kept by the ATM with the help of an RTC device.

4. **Card Reader** : The card reader is an input device that reads data from a card. The card reader is part of the identification of your particular account number and the magnetic strip on the backside of the ATM card is used for connection with the card reader. The card is swiped or pressed on the card reader which captures your account information i.e. the data from the card is passed on to the host processor (server). The host processor thus uses this data to get the information from the cardholders.

5. **Receipt Printer** : The receipt printer prints all the details recording your withdrawal, date and time, and the amount of withdrawal and also shows the balance of your account in the receipt.

### ATM Networking

The internet service provider (ISP) also plays an important role in the ATMs. This provides communication between ATM and host processors. When the transaction is made, the details are input by the cardholder. This information is passed on to the host processor by the ATM. The host processor checks these details with an authorized bank. If the details are matched, the host processor sends the approval code to the machine so that the cash can be transferred.
