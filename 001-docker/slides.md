## Improving developer experience (DX) with Docker

---

## Docker's Awakening DX
 
---


## The Legend of /(/(n((n/)))): DX

According to Aaron (1.5 years old)

---

## Dustin Masters

Senior Software Engineer, Olo

---

![](7.png)

---

## See also:

- https://ReactJS.NET
- https://woke.dev

---

## Slow builds are the WORST

Note: Team uses OS X Primarily. Can we make the Windows builds better?

---

## Rebuilds took over 6 seconds on average between changes 🐢

When not running as admin, could be as slow as 30 seconds, because symlinks..

---


## Javascript builds access lots of files

---

![](3.png)

---

## Root problem

Our Ember build creates a _lot_ of temporary files

---

## Filesystem access on Windows can be slow

Even with WSL, NTFS is still used behind the scenes via DrvFs


---

https://github.com/Microsoft/WSL/issues/873

![](4.png)
![](5.png)

---

![](https://media.giphy.com/media/26ybwvTX4DTkwst6U/giphy.gif)

---


## What if we used the blockchain?

---

🚫

---


## What if we used containers?

---

✅

---

## Perf test on a VM

Native: 78s build, 6s rebuild

Container: 45s build, 2s rebuild

---

## Other benefits

- Consistent build environment
- Multiple containers can be linked

---

## New problem: Keeping the files in sync

Docker does not notify mapped volumes that data has changed

---

## Dotnet Tool to the rescue

https://github.com/dustinsoftware/Docker-Volume-Watcher

`dotnet install --global DockerVolumeWatcher`

---

## Automation is 🔑

`yarn docker-start` boots up all the containers and does sanity checks

![](6.png)

---

## Thanks!

@dustinsoftware 🐤

---

## Credits
- `reveal-md`
- `dotnet tool`

