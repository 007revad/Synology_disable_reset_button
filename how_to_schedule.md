# How to schedule a script in Synology Task Scheduler

To schedule a script to run on your Synology follow these steps:

**Note:** You can setup a schedule task and leave it disabled, so it only runs when you select the task in the Task Scheduler and click on the Run button.

Schedule **toggle_reset_button.sh disable** to run at boot:

1. Go to **Control Panel** > **Task Scheduler** > click **Create** > and select **Triggered Task**.
2. Select **User-defined script**.
3. Enter a task name like Disable Reset Button.
4. Select **root** as the user (The script needs to run as root).
5. Select **Boot-up** as the event that triggers the task.
6. Leave **Enable** ticked.
7. Click **Task Settings**.
8. Optionally you can tick **Send run details by email** and **Send run details only when the script terminates abnormally** then enter your email address.
9. In the box under **User-defined script** type the path to the script. 
    - e.g. If you saved the script to a shared folder on volume 1 called scripts you'd type:
    - **/volume1/scripts/toggle_reset_button.sh disable**
10. Click **OK** to save the settings.


Schedule **toggle_reset_button.sh enable** to run manually:

1. Go to **Control Panel** > **Task Scheduler** > click **Create** > and select **Scheduled Task**.
2. Select **User-defined script**.
3. Enter a task name like Enable Reset Button.
4. Select **root** as the user (The script needs to run as root).
5. Select **Boot-up** as the event that triggers the task.
6. Untick **Enable**.
7. Click **Task Settings**.
8. Optionally you can tick **Send run details by email** and **Send run details only when the script terminates abnormally** then enter your email address.
9. In the box under **User-defined script** type the path to the script. 
    - e.g. If you saved the script to a shared folder on volume 1 called scripts you'd type:
    - **/volume1/scripts/toggle_reset_button.sh enable**
10. Click **OK** to save the settings.

