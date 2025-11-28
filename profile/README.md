# Beacon: A gateway to freedom tech

Lighting in WhatsApp (Video Demo)
https://primal.net/e/nevent1qqsq5uap9tj235xayy49zmtwwc6yk3h3yxpyecg03kue6g5a6seze2ckr0xdv
https://blossom.primal.net/f56be68b58aa87cf0006d6d2fc69a59e8d6e4b36a73efa31de547ce53569873f.mp4

Onboarding (Video Demo Live at Sov Eng!)
https://r2a.primal.net/uploads2/8/31/50/8315018b9b601d17269e36a7aa82c98370bf285be8ea741ff60da8c923220a4c.mov

## Why Beacon? 

> On the island of Pharos the Ptolemies lit a beacon that turned Alexandria into the nerve-centre of the ancient world, guiding mariners safely into the port of liberty, knowledge and freedom. 
> With free access to information we can find our own solutions and build our own freedom. The library of Alexandria once represented this freedom but was lost to time. 
> The goal of the project is to relight a similar flame on the internet. To take closed, controlled networks and guide people towards free information, free networks and freedom money.

Beacon is intended as an open standard to allow a market of service providers to offer access to bitcoin lightning wallets and various freedom tech services, with no on device install and minimal barrier to entry inside the applications and chat networks you already use.

Beacon was born out of an initial frustration when trying to deliver sophisticated apps in places where the regular user couldn't afford internet, the internet was bad when they did have it and smartphones barely existed. 

The one thing that always work reliably however, was WhatsApp. So the idea was to hijack WhatsApp (and other networks including signal, telegram, nostr dm, text, mesh) and put the wallet into the chat using an AI chatbot to orchestrate tasks. 

WhatsApp is not an ideal chat network and we wouldn't want people stuck their long term, so all new users bootstrap a full Nostr account and profile and Nostr Wallet Connect for wallet management, reducing lock in and offering a pragmatic onboarding flow from WhatsApp to full sovereign Nostrich and Bitcoiner. 

Beacon is not to be "the wallet to end them all" it is to provide a pragmatic entry point.

A trojan horse for freedom tech.

## The Trust Model

This is based on a two factor approach. Two seperate services are combined to run a Beacon, the ID and the Brain.

The concept is one where you could have 1000's to Millions of ID servers and 10-100s of Brains. 

The ID server holds the important pieces - your key and signs off on and approves any spends or signs events for Nostr. You can even self host and bring your own ID server by running a simple app (no internet routing config required) on a simple Raspi or alterative. 

The Brain does the heavy lift, it will examines the incoming messages, understands the intent of what you are trying to achieve and allows you to undertake complex interactions, all through a chat interface. This requires access to AI models and is more complex to run. The expectation here is that a small market of providers can sell AI services here to sell AI services and Information to an otherwise captive market. Critically the Brain provider and the ID provider do not need to know each other, the user chooses the two service providers and makes the link via pubkeys. 

<img width="1038" height="905" alt="image" src="https://github.com/user-attachments/assets/10afab7a-c620-4895-b8d4-33d5db47ee9a" />

A novel concept used in the app is to take what would usually be a single custodial service and split it into multiple parts all connected over Nostr. This has a direct impact on the trust model as suddenly you can run the most component of the app, the signing of messages that approve spend or identity action, seperately to your main business logic. This allows a service provider to offer a complex service like running AI models without hold the key. 

The key can instead be held at the personal, family, community or business level. 

## Target Networks

So far we have had success running Beacon on WhatsApp continually and have had working prototypes on Signal, Qual (mesh) and Nostr DMs. We are keen to expand on this and have a pluaggable gateway to allow devs to create new adaptors to a simple REST and SSE interface. 

The goal is no more walled gardens, Bitcoin everywhere and everyone gets an Npub. 

![freedom_tech_meme](https://github.com/user-attachments/assets/622123cc-86e0-4365-9bbf-73d2ffe56685)
