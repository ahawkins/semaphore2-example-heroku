# Semaphore and Herkou Example

This small example repo demonstrates how to trigger Heroku deploys
from Semaphore builds. Feel free to fork or copy and paste from this
example. Setup is straight forward:

1. Create your Heroku API key. You can do this via the Heroku CLI:
   `heroku authorizations:create`
2. Set that value in `secret.yml` then create the secret with sem:
   `sem create -f secret.yml`. Remove `secret.yml` from source control
   at this point.
3. Set your app name in `.semaphore/semaphore.yml`
4. Push
5. Done!

Once your deploy step is working, you can configure an automatic or
manual promotion to different Heroku applications.
