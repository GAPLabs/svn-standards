STANDARD 2
==========

### Naming Conventions ###



Release Branch
--------------

Release branch names must start with `rb`, followed by a dash/minus (`-`), followed by the major version number, followed by a dot (`.`), followed by the minor version number. Minor version numbers start from zero for every major version.

               +--------+   +--------+   +--------+
               | rb-1.0 |   | rb-1.2 |   | rb-2.1 |
               +--------+   +--------+   +--------+
              /             /             /
             /             /             /
            /             /             /
    Trunk -+------+------+------+------+------------------>
                   \             \                   
                    \             \
                     \             \
                      +--------+   +--------+
                      | rb-1.1 |   | rb-2.0 |
                      +--------+   +--------+



Feature Branch
--------------

Feature branch names must start with `fb`, followed by a dash/minus (`-`), followed by the feature name, and optionally followed by a version number.

               +-----------+
               | fb-review |
               +-----------+
              /             \
             /               \
            /                 \
    Trunk -+--------+----------+--+---+------------------->
                     \             \ /                   /
                      \             X                   /
                       \           / \                 /
                        +---------+   +---------------+
                        | fb-ajax |   | fb-review-1.1 |
                        +---------+   +---------------+



Task Branch
-----------

Task branch names must start with `tb`, followed by a dash/minus (`-`), followed by a task id.

               +------+      +------+
               | tb-1 |      | tb-3 |
               +------+      +------+
              /        \    /        \
             /          \  /          \
            /            \/            \
    Trunk -+------+------++-----++------+------+---------->
                   \            /\            /
                    \          /  \          /
                     \        /    \        /
                      +------+      +------+
                      | tb-2 |      | tb-4 |
                      +------+      +------+



Experimental Branch
-------------------

Experimental branch names must start with `try`, followed by a dash/minus (`-`), followed by the experiment name, and optionally followed by a version number.

               +----------+
               | try-php5 |
               +----------+
              /            \
             /              \
            /                \
    Trunk -+---+--------------+---+----------------------+>
                \                  \ /                  /
                 \                  X                  /
                  \                / \                /
                   +--------------+   +--------------+
                   | try-backbone |   | try-php5-1.1 |
                   +--------------+   +--------------+



Release Tag
-----------

Release tag names must start with `rel`, followed by a dash/minus (`-`), followed by the version number of its corresponding release branch, followed by a dot (`.`), followed by the release number. Release numbers start from zero for every release branch.

    Trunk --+--------------------------------------------->
             \                    +------+
              \                   | tb-1 |
               \                  +------+
                +--------+       /        \
                | rb-1.0 |--+---+----------+---+---------->
                +--------+  |                  |
                            |                  |
                            |                  |
                      +-----+-----+      +-----+-----+
                      | rel-1.0.0 |      | rel-1.0.1 |
                      +-----------+      +-----------+

