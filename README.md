# Server: Auto Stop

Save the server cost by shutting down the server after 60 minutes of inactivity.

*IMPORTANT NOTE*

Not all server provider frees the stopped instance, and most still charge for
the data disk. Please check with your server provider about the charging scheme.

## Setup

1. Clone this GIT repository.

   ```sh
   git clone https://github.com/cytim/server.auto-stop.git auto-stop
   ```

2. Setup the crontab (under the `root` user).

   ```ssh
   crontab -e
   ```

   ```sh
   * * * * * /PATH/TO/THE/AUTO_STOP/PROJECT/main
   ```

