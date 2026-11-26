# Oracle Database 11g Architecture

**For the single-instance course, open [Oracle Database 11g Stand-Alone Architecture](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/stand-alone-db.html).** It contains all **57 workflows** for Oracle Database 11g R2 (11.2.0.4) in one HTML file.

1. Select **Browse all 57 workflows** near the top of the page to see every lesson title grouped into 11 operation categories. Select a title to open its manual guide, then choose **Next step** to begin.
2. To save an offline copy, choose **Download this HTML** on the trainer page. Open the downloaded HTML file in your browser. The diagrams, playback controls, and checkpoints work offline. The Oracle documentation links open online.
3. If you previously used v77, look under **Startup / Shutdown / Recovery** for shutdown NORMAL, TRANSACTIONAL, and ABORT with recovery. Under **Database Patching & Upgrades** you will find six lessons covering quarterly patching, one-offs, Windows bundles, patch-set upgrades, rollback, and upgrade-mode failure diagnosis.

To move between Stand-Alone DB and the five specialist towers, use the [six-tower course home](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/).

## A first session

1. Search for **User Login / Session Creation** and choose **Manual Demo**. Select **Next step** to follow the client from its connection request to an authenticated session.
2. Try **First-Time SELECT / Hard Parse**, then **INSERT + COMMIT**. Watch which process handles the SQL and which process makes a normal commit durable.
3. At the final step, answer the question in your own words and expand **Suggested answer** to compare. Use **Reset timeline** to replay the steps or the reset button beside the diagram to choose another workflow.

## Use the controls in any tower

1. Choose a tower at the top of the page. In the workflow explorer, filter by **operation category** or **difficulty**, or enter a workflow name in the search box.
2. Choose **Manual Demo** to read the workflow guide. Press **Next step** in the bottom player to see the first step in the diagram. Choose **Auto Demo** on a workflow card to start playback immediately.
3. Use **Play**, **Pause**, **Previous step**, and **Next step** to control the animation. Change the speed, turn **Loop Flow** on to repeat, or select a named step on the timeline to revisit it. You can also drag the slider to a step. On phones the active player stays at the bottom of the screen. **Reset timeline** takes you back to the start of the selected workflow.
4. Search for a component beside the diagram, or select it in the drawing to inspect its role. On Stand-Alone DB, try **LGWR** during a commit. On RAC, try **SCAN listener** during a client connection.
5. Use the diagram’s full-screen control for a closer look. Open **References** in the top toolbar to consult the Oracle documentation for that tower.

## Follow a change through the architecture

The database examples use **Oracle Database 11g Release 2 (11.2.0.4)**. GoldenGate uses the 11.2.1 Classic architecture. Enterprise Manager uses Cloud Control 12.1 with an 11g database target.

The links below open individual workflows. Look for the highlighted components and connections as you advance. With reduced motion enabled, these highlights still identify the current step.

| Start here | Follow on the diagram |
|---|---|
| [RAC · retrieve a remote consistent-read block](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/rac.html#rac-7) | Follow a block from the peer cache across the private interconnect. Replay the shared-storage case. |
| [Data Guard · follow one commit](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/dataguard.html#dg-1) | Identify local redo durability, receipt in the standby redo log, and application to standby data files. |
| [RAC + Data Guard · follow a block and redo](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/rac-dataguard.html#both-1) | Locate the block transfer inside the cluster and the separate redo path to the other site. |
| [GoldenGate · trace a committed change](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/goldengate.html#trace-a-commit) | Follow Extract, the local trail, the data pump, the remote trail and Replicat into the target database. |
| [Enterprise Manager · follow the first sample](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/oem.html#first-sample) | Follow a target observation through the Management Agent and OMS to the repository and console. |

## Compare a workflow across technologies

1. On the home page, expand **Compare a home workflow across the five towers** and choose any workflow. Each row explains whether the lesson carries over directly, changes with the topology, supplies background, or falls outside that tower’s lessons.
2. Choose **Open lesson** in a matching row. For example, compare **INSERT + COMMIT** in a physical standby configuration with the committed transaction that GoldenGate captures and delivers to its target. On the tower page, expand **Related Stand-Alone DB workflows** to return to a specific foundation lesson.
3. For operations, follow **Startup**, **Graceful shutdown**, and **Patching** in each tower. Use the starting conditions to identify which instance, site, product home, or service the maintenance affects. Answer the final checkpoint using the evidence from that topology.

## Practice database operations on the home page

On **Stand-Alone DB**, use the **All operation categories** dropdown to find a workflow. Select **Startup / Shutdown / Recovery** for startup and shutdown, or **Database Patching & Upgrades** for patching. On the workflow card, choose **Manual Demo**, then **Next step**.

1. **Startup.** Open **Instance Startup / NOMOUNT, MOUNT and OPEN**. At each stage, identify which files Oracle has opened and what the administrator can verify.
2. **Graceful shutdown.** Run **Graceful Shutdown / NORMAL**, **TRANSACTIONAL**, and **IMMEDIATE**. Compare what Oracle waits for, who disconnects sessions, and how the database closes. The separate **Shutdown ABORT / Recovery on Next Startup** lesson shows what recovery must do after an abrupt stop.
3. **Patching.** Start with **Quarterly Database Patching / PSU and SPU**. Follow the selected Oracle home, inventory, required database SQL actions and application test. Continue with the one-off, Windows bundle, patch-set upgrade, rollback and upgrade-failure lessons.

## Choose a tower

| Tower | Start with this question |
|---|---|
| [Stand-Alone DB](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/) | How does a single instance open, execute work, commit, and close? |
| [RAC and Grid Infrastructure](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/rac.html) | How do two instances serve one database? |
| [Data Guard](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/dataguard.html) | When has a standby received a change, and when has it applied it? |
| [RAC + Data Guard](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/rac-dataguard.html) | Which failures can a cluster handle locally, and which can lead to a database role change? |
| [GoldenGate](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/goldengate.html) | How does a committed change reach a separate target through trail files? |
| [Enterprise Manager](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/oem.html) | How does an observation from a managed target reach the monitoring console? |

## Use all six trainers offline

1. Open the GitHub file links below. On each file page, choose **Download raw file**.
2. Save all six HTML files in one folder using the displayed filenames: [index.html](index.html), [rac.html](rac.html), [dataguard.html](dataguard.html), [rac-dataguard.html](rac-dataguard.html), [goldengate.html](goldengate.html), and [oem.html](oem.html).
3. Open **index.html** in your browser. The tower links use these sibling filenames. External Oracle reference links need an internet connection.
4. If you also want the course home's **Open the Stand-Alone DB single-file edition** link to work offline, save [stand-alone-db.html](stand-alone-db.html) beside **index.html** using the filename **stand-alone-db.html**.
