# REPley Ride beta

Indoor riding on your smart trainer, with calm scenery and your own videos alongside. Free while we
test it. You sign in to REPley Ride with your email: it sends you a code to type in.

## What you need

- A smart trainer that speaks Bluetooth FTMS, the standard most recent trainers use. The beta is
  untested on most models, so tell us how yours goes.
- A computer with Bluetooth: a Mac, a Windows 10 or 11 PC, or a Linux computer.
- A heart-rate strap if you have one. It is optional.

## 1. Download

| Your computer | Download |
|---|---|
| Mac with an Apple chip (M1 or later) | [REPley-Ride-mac-apple-silicon.dmg](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-mac-apple-silicon.dmg) |
| Mac with an Intel processor | [REPley-Ride-mac-intel.dmg](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-mac-intel.dmg) |
| Windows 10 or 11 | [REPley-Ride-windows.exe](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-windows.exe) |
| Linux | [REPley-Ride-linux.AppImage](https://github.com/Matt-Crofts/repley-ride-releases/releases/latest/download/REPley-Ride-linux.AppImage) |

Not sure which Mac you have? Choose Apple menu > About This Mac: it says **Chip: Apple M…** for an Apple chip, or
**Processor: Intel** for Intel. Each Mac download carries only what that chip needs, so it is about 100 MB smaller than
one for both.

These links always give the newest version. Every download's checksum is in `SHA256SUMS` on the release.

## Versions

| Version | Released |
|---|---|
| **0.5.2** (newest) | 3 Oct 2026, 9:38 AM |
| 0.5.1 | 2 Oct 2026, 10:15 PM |
| 0.5.0 | 2 Oct 2026, 5:39 PM |
| 0.4.3 | 30 Sep 2026, 8:56 PM |
| 0.4.2 | 30 Sep 2026, 8:08 PM |
| 0.4.1 | 30 Sep 2026, 8:05 AM |
| 0.4.0 | 30 Sep 2026, 1:28 AM |
| 0.3.0 | 29 Sep 2026, 7:45 AM |
| 0.2.1 | 28 Sep 2026, 10:15 PM |
| 0.2.0 | 28 Sep 2026, 5:34 PM |

The newest is at the top, with when it came out (Melbourne time). When a newer version than yours is out,
REPley Ride says so on its start screen, with a link back here.

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

## 3. Sign in

The first time REPley Ride opens, it asks for your email, then for the code it sends you. Your REPley
account is how the beta knows you: use the same email on each computer.

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
Linux, replace the old file. If you paired with REPley on a beta build from before 0.2.1, your Mac asks
once, when you next pair or a ride is sent, whether REPley Ride may use its keychain: click **Always Allow**.
Builds from 0.2.1 on are signed, so they are never asked again.

## Your data

While you are in the beta, the app tells us when you ride, for how long and how far, the scene and
mode, your trainer's model, your computer's system and the app version, so we can see what riders
use. After a ride on a trainer, or a start that fails, it also sends that session's Bluetooth log:
when your trainer and strap connected and dropped and what went wrong, so we can fix it. Never
your heart rate or power: your rides stay on your computer unless you send them to REPley or
Strava.

So that we can tell testers apart, and answer you, we keep the first name and email from your REPley
account next to those reports.

## Help

Stuck, or found something broken? Tell whoever sent you this page.
