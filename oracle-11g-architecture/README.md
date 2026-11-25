# Oracle Database 11g Architecture

[Open the Stand-Alone DB page](https://jones4u.github.io/oracle-database-architecture/oracle-11g-architecture/). Start here for single-instance lessons or choose a tower from the navigation. Each tower links back to the Stand-Alone DB page.

## A first session

1. Search for **User Login / Session Creation** and choose **Manual Demo**. Select **Next step** to follow the client from its connection request to an authenticated session.
2. Try **First-Time SELECT / Hard Parse**, then **INSERT + COMMIT**. Watch which process handles the SQL and which process makes a normal commit durable.
3. At the final step, answer the question in your own words and expand **Suggested answer** to compare. Use **Reset timeline** to replay the steps or the reset button beside the diagram to choose another workflow.

To explore a component on its own, use the diagram search. Search for **LGWR**, for example, to read what the log writer does during a commit.

## Compare a workflow across technologies

1. On the home page, expand **Compare a home workflow across the five towers** and choose any workflow. Each row explains whether the lesson carries over directly, changes with the topology, supplies background, or falls outside that tower’s lessons.
2. Choose **Open lesson** in a matching row. For example, compare **INSERT + COMMIT** in a physical standby configuration with the committed transaction that GoldenGate captures and delivers to its target. On the tower page, expand **Related Stand-Alone DB workflows** to return to a specific foundation lesson.
3. For operations, follow **Startup**, **Graceful shutdown**, and **Patching** in each tower. Use the starting conditions to identify which instance, site, product home, or service the maintenance affects. Answer the final checkpoint using the evidence from that topology.

## Practice database operations on the home page

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
