# action-repo

This repository is monitored by GitHub webhooks. All pushes, pull requests, and merges trigger webhook events that are captured and displayed in real-time.

## Purpose

This repository serves as the **action-repo** for the GitHub Webhook Integration assignment. It's configured to send webhook events to the webhook receiver application.

## Monitored Actions

- **Push**: When code is pushed to any branch
- **Pull Request**: When a pull request is opened or reopened
- **Merge**: When a pull request is merged

## Webhook Endpoint

All events are sent to: `https://convoluted-plasticly-elvia.ngrok-free.dev/webhook`

## How It Works

1. Any push, pull request, or merge in this repository triggers a webhook
2. GitHub sends the event data to the webhook endpoint
3. The webhook receiver stores the event in MongoDB
4. The UI displays the event in real-time

## Testing

Make changes to this repository:
- Push commits to test push events
- Create pull requests to test PR events
- Merge pull requests to test merge events

Check the webhook receiver UI to see all events!

## Links

- **Webhook Receiver**: https://github.com/Kaustubhpatel11/webhook-repo
- **Live UI**: https://convoluted-plasticly-elvia.ngrok-free.dev
