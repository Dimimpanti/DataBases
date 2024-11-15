# Application Overview

## 1.1 Σκοπός της εφαρμογής

Η εφαρμογή στοχεύει στη διαχείριση και παρακολούθηση ενός έξυπνου σπιτιού μέσω ενός δικτύου αισθητήρων που ανιχνεύουν περιβαλλοντικές συνθήκες και καταστάσεις, όπως η αύξηση της θερμοκρασίας και μιας υβριδικής συσκευής (π.χ., smartwatch). Οι αισθητήρες αυτοί, σε συνδυασμό με το υβριδικό σύστημα, ενεργοποιούν τις κατάλληλες συσκευές ώστε να διατηρούν το περιβάλλον στις ιδανικές συνθήκες που έχει ορίσει ο χρήστης ανάλογα με τις προτιμησεις του.

Με αυτό τον τρόπο, εξασφαλίζεται τόσο η ασφάλεια του σπιτιού (π.χ., μέσω του συστήματος συναγερμού και του αυτόματου ποτίσματος του κήπου) όσο και η ευημερία του κατοίκου. Το σύστημα μπορεί να παρακολουθεί και να προσαρμόζει συνθήκες που επηρεάζουν τη βιωσιμότητα και την ποιότητα ζωής του χρήστη, όπως η θερμοκρασία και ο φωτισμός, προσφέροντας έτσι έναν έξυπνο, ασφαλή και υγιή χώρο διαβίωσης.


## 1.2	Περιγραφή Εφαρμογής

Η εφαρμογή προσφέρει στον χρήστη τη δυνατότητα να παρακολουθεί τη φυσική του κατάσταση μέσω του smartwatch του, αποθηκεύοντας δεδομένα που αφορούν την υγεία του (όπως παλμοί, θερμίδες, βήματα κ.λπ.). Επιπλέον, ο χρήστης ενημερώνεται μέσω notifications από το smartwatch για τις προγραμματισμένες του δραστηριότητες, ώστε να παραμένει οργανωμένος και "on track" με το καθημερινό του πρόγραμμα.
Παράλληλα, η εφαρμογή του δίνει τη δυνατότητα να ρυθμίζει και να ελέγχει διάφορες συσκευές του σπιτιού (όπως φωτισμό, θερμοκρασία και σύστημα συναγερμού) βάσει των προσωπικών  προτιμήσεων που έχει θέσει. 



- **User Entity**: Each user has a unique ID. Users also have an assigned role within the home (e.g., admin, guest, child) that defines their access level to different devices. 
   - **Admin**: Has full access to configure devices and set rules.
   - **Guest**: Limited access, primarily for monitoring or basic usage.
   - **Child**: Restricted access, tailored for a safe and controlled environment.

### Devices, Sensors, and Actuators
- **Devices**: This includes all smart home components, such as sensors and actuators, which are designed to monitor and control the home environment. 
- **Sensors**: These are responsible for observing conditions within the home, like temperature, humidity, or light levels. Based on specific **trigger conditions** (e.g., a drop in temperature below a set threshold) set by the admin, sensors activate actuators to respond to changes in the environment.
- **Actuators**: When triggered, actuators perform specific actions, such as adjusting the temperature or turning on lights, to ensure a comfortable and safe environment. This interconnected system provides automation and real-time responses to ensure the home remains secure and optimally managed at all times.

### Smartwatch Integration
- **Smartwatch**: The smartwatch is a dedicated device within the system, responsible for tracking user health metrics (e.g., step count, heart rate). It also sends notifications for scheduled activities, helping users stay on track with their routines and promoting a healthy lifestyle.

## Safety and Security

This database setup not only provides convenience but also enhances safety within the home. By allowing admins to set conditions and automate responses (such as activating security systems when certain triggers are met), the application helps prevent unsafe situations and ensures that access to devices is controlled according to each user’s role.

## Example Usage

Imagine a user who wants to automate their smart home and maintain a healthy routine:
1. **Roles and Access**: The user has an admin role, allowing them to configure devices and set triggers. They can manage which users (e.g., guests, children) have access to specific devices.
2. **Setting Trigger Conditions**: The admin sets a trigger on a temperature sensor to activate the heating system if the temperature drops below 18°C, ensuring comfort and safety.
3. **Health and Reminders**: The user’s smartwatch tracks their daily steps and heart rate, sending reminders for activities like exercise or taking breaks. This helps the user stay on top of their health and daily schedule.

