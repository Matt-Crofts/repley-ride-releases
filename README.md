# REPley Ride beta

Indoor riding on your smart trainer, with calm scenery and your own videos alongside. Free while we
test it. You need an invite code; it came with your invite.

## What you need

- A smart trainer that speaks Bluetooth FTMS, the standard most recent trainers use. The beta is
  untested on most models, so tell us how yours goes.
- A computer with Bluetooth: a Mac, a Windows 10 or 11 PC, or a Linux computer.
- A heart-rate strap if you have one. It is optional.

## 1. Download

| Your computer | Download |
|---|---|
| Mac (Apple chip or Intel) | [REPley-Ride-mac.dmg](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-mac.dmg) |
| Windows 10 or 11 | [REPley-Ride-windows.exe](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-windows.exe) |
| Linux | [REPley-Ride-linux.AppImage](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-linux.AppImage) |

These links always give the newest version. Every download's checksum is in `SHA256SUMS` on the release.

## 2. Install

**Mac**
1. Open the downloaded file and drag REPley Ride into Applications.
2. Open REPley Ride from Applications. It is signed and checked by Apple, so it opens straight away.
3. When REPley Ride asks to use Bluetooth, click **Allow**.

**Windows**
1. Open the downloaded file. The beta is not yet registered with Microsoft, so if Windows says it
   protected your PC, click **More info**, then **Run anyway**. REPley Ride installs and opens.
2. Make sure Bluetooth is on in Settings, Bluetooth & devices. Windows has had the least testing so
   far, so tell us how it goes.

**Linux: Arch and Omarchy**

Add the REPley Ride repository once, then install it like any other package. It appears in the app menu, and
`sudo pacman -Syu` updates it with everything else.

```bash
sudo tee -a /etc/pacman.conf >/dev/null <<'EOF'

[repley-ride]
SigLevel = Optional TrustAll
Server = https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download
EOF
sudo pacman -Sy repley-ride-bin
```

The packages are built from a public recipe (`repley-ride-bin-recipe.tar.gz` on each release) and are not signed
yet, which is what the `SigLevel` line allows for.

**Other Linux**
1. Make the file runnable: in a terminal, `chmod +x ~/Downloads/REPley-Ride-linux.AppImage`
   (or in your file manager: Properties, then allow it to run as a program).
2. Open it.

## 3. Join with your code

The first time REPley Ride opens, type the invite code from your invite and click **Join the beta**.
Each computer needs it once.

## 4. Set up and ride

1. On **Your rider**, set your weight, then pedal to wake your trainer and choose it. Choose your
   heart-rate strap too, if you have one, and wet its electrodes before you ride.
2. Click **Next**, then **Start ride**. No trainer to hand? **Ride with the simulator** to look around.
3. During a ride, press **?** to see the keys.

Close Zwift, the Wahoo app or any other training app first: only one app at a time can control the
trainer.

After your first ride, REPley Ride asks two quick questions. Your answers shape what we build next.

## Updates

When a new version is ready, the start screen says so. Download it from this page and install it
over the old one: on a Mac, drag it into Applications again; on Windows, open the new installer; on
Linux, replace the old file. On a Mac, if you connected REPley Ride to REPley, the update may ask
whether it can use its saved connection: click **Always Allow**.

## Your data

While you are in the beta, the app tells us when you ride, for how long and how far, the scene and
mode, your trainer's model, your computer's system and the app version, so we can see what riders
use. Never your heart rate or power: your rides stay on your computer unless you send them to
REPley or Strava.

## Help

Stuck, or found something broken? Reply to the message your invite came in.
