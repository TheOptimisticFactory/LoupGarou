## Fork of leomelki/LoupGarou by TheOptimisticFactory

- This repository is based off https://github.com/leomelki/LoupGarou and contains improvements made by the community before it lands in the main repository (if ever).
- The `dev` branch is **STABLE**, despite his name. The `wip` branch, on the other hand might not

## Useful commands (for ops) ##

- `/lg joinAll` to make everyone connected join the lobby
- `/lg start` to start the game
- `/lg end` to interrupt an ongoing game
- `/lg nick <username> <nickname>` to set a nickname to a player
- `/lg addSpawn` to add a spawn-point on your EXACT position and look direction
- `/lg roles` to get the list of currently active roles
- `/lg roles list` to get the complete list of available roles
- `/lg roles set <role> <amount>` to set the number of players for a given role

## Notes ##

- The following warning is normal and can safely be ignored: `WARNING: Illegal reflective access by com.comphenix.net.sf.cglib.core.ReflectUtils$1 (file:<path>) to method java.lang.ClassLoader.defineClass(java.lang.String,byte[],int,int,java.security.ProtectionDomain)`. It is due to the fact that [ProtocolLib currently does not support Java versions above Java 8 and won't until Mojang and Spigot decide to update.](https://github.com/dmulloy2/ProtocolLib/issues/603#issuecomment-490207994)

## Additional features compared to original plugin ##

#### 01) Village composition showcase at the end of the game

- https://github.com/leomelki/LoupGarou/pull/42 (Author: [TheOptimisticFactory](https://github.com/TheOptimisticFactory))

  ![image](https://user-images.githubusercontent.com/2607260/79672340-4260a780-81d1-11ea-9b49-266a992e872a.png)

#### 02) Ability to set nickanmes to players

- https://github.com/leomelki/LoupGarou/pull/40 (Author: [Nicooow](https://github.com/Nicooow)).
- Tweaked the PR with an [additional commit (9cbb739)](https://github.com/TheOptimisticFactory/LoupGarou/commit/9cbb73935532cacab8787cc4586a64e42b65958e) to:
  + support nickname containing spaces
  + color the nicknames

  ![image](https://user-images.githubusercontent.com/2607260/79674319-56f96b80-81e2-11ea-87ef-d4bdfd4494aa.png)

  ![javaw_Nk1NdY7KXw](https://user-images.githubusercontent.com/2607260/79673723-8e651980-81dc-11ea-8258-eb077bca7fca.png)

#### 03) GUI to configure roles and start game

- https://github.com/leomelki/LoupGarou/pull/19 (Author: [Commantary](https://github.com/Commantary)).
- Tweaked the PR with an [additional commit (7df0439)](https://github.com/TheOptimisticFactory/LoupGarou/commit/7df04392ecb443d42207b859fcbbf4188e8080ae) to:
  + fix compilation issues

  ![image](https://user-images.githubusercontent.com/2607260/80097236-41ca6700-856b-11ea-978c-dd658ad09c67.png)

#### 04) Highlight of the % of votes on a given player

- https://github.com/leomelki/LoupGarou/pull/43 (Author: [TheOptimisticFactory](https://github.com/TheOptimisticFactory))

  ![image](https://user-images.githubusercontent.com/2607260/79676799-f706c300-81e9-11ea-86cd-0c9cd98be0b3.png)

#### 05) Server logs when a player dies or gets resurrected

- https://github.com/leomelki/LoupGarou/pull/47 (Author: [TheOptimisticFactory](https://github.com/TheOptimisticFactory))

  ![image](https://user-images.githubusercontent.com/2607260/80264401-56564e80-8694-11ea-9f28-89a425b4d59b.png)

#### 06) Revamped scoreboard to avoid useless scoring

- Needs testing before the PR gets created. (Author: [TheOptimisticFactory](https://github.com/TheOptimisticFactory))
  + Added highlight of the total number of players remaining.
  + Added support of plural names in the scoreboard.
  + Rewritten logic to avoid instantiating 15 instances when 1 is sufficient.

  ![javaw_wQKF2n7IGS](https://user-images.githubusercontent.com/2607260/80265125-c5cd3d80-8696-11ea-8e32-0d1fc49d5708.png)
