STANDARD 1
==========

### Structure ###



Trunk
-----

The trunk contains development code that will be on the next major release.

No actual development will occur on the trunk. Instead, development will be on branches then merge back into trunk.

    Trunk ------------------------------------------------>



Branches
--------

Branches are copies of the trunk or other branches that can generally be used for development.



### Release ###

Release branches are created when the trunk reaches a stage where it’s ready to be released. This branch contains code that will be on the next release of this branch.


    Trunk ---+-------------------------------------------->
              \               
               \             
                \           
                 +--------+
                 | rb-x.y |
                 +--------+


### Feature ###

Feature branches are for isolating new features which may otherwise destabilize the Trunk in the course of its development. When the feature is completed, this branch is merged back into the trunk.

    Trunk ---+----------------+--------------------------->
              \              /
               \            /
                \          /
                 +--------+
                 | fb-x.y |
                 +--------+


### Task ###

Task branches are typically short-lived branches for development tasks leading/contributing to the next major release. When the task is completed, this branch is merged back to the trunk and deleted.

    Trunk ---+--------------+----------------------------->
              \            /
               \          /
                \        /
                 +------+
                 | tb-x |
                 +------+


### Experimental (new) ###

Experimental branches are for isolating the introduction of new technologies. For example, legacy codebase has to be rewritten from PHP 4 to PHP 5. If the experiment succeeds, the branch is then merged into the trunk.

    Trunk ---+----------------------+--------------------->
              \                    /
               \                  /
                \                /
                 +--------------+
                 | try-NAME-x.y |
                 +--------------+



Tags
----

Tags are copies of branches that are not used for development. Tags only serve to mark a certain state of a branch.



### Release ###

A release tag is a copy of a release branch ready to go live. Basically, every release tag is a copy of a release branch version that has gone live.

    Trunk ---+-------------------------------------------->
              \               
               \             
                \           
                 +--------+
                 | rb-x.y |--------+---------------------->
                 +--------+        |
                                   |  # Tagged!
                                   |
                             +-----+-----+
                             | rel-x.y.z |
                             +-----------+

