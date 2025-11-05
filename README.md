# Deploy n8n on Render

> [!IMPORTANT]
> **View full deployment instructions in the [**Render docs**](https://render.com/docs/deploy-n8n).**

This template defines a [`render.yaml`](https://github.com/render-examples/n8n/blob/main/render.yaml) file you can use to deploy [n8n](https://n8n.io/) on Render. Click **Use this template** in the upper right to copy this template into your account as a new repo.

The `render.yaml` file defines the following resources:

- A web service that pulls and runs the official n8n Docker image
- A Render Postgres database that stores n8n data

Each of the above uses a free instance type by default.

Important: Keep It Alive (For free render users)
Free tier sleeps after 15 mins of inactivity. To keep it awake:​

Setup Cron Job:

Go to https://cron-job.org (free account)​

Create new cron job:

URL: https://your-n8n-xyz.onrender.com

Schedule: Every 10 minutes (*/10 * * * *)​

Save → Your n8n stays awake 24/7​
