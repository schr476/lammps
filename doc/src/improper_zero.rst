.. index:: improper\_style zero

improper\_style zero command
============================

Syntax
""""""


.. parsed-literal::

   improper_style zero *nocoeff*

Examples
""""""""


.. parsed-literal::

   improper_style zero
   improper_style zero nocoeff
   improper_coeff \*

Description
"""""""""""

Using an improper style of zero means improper forces and energies are
not computed, but the geometry of improper quadruplets is still
accessible to other commands.

As an example, the :doc:`compute improper/local <compute_improper_local>` command can be used to
compute the chi values for the list of quadruplets of improper atoms
listed in the data file read by the :doc:`read\_data <read_data>`
command.  If no improper style is defined, this command cannot be
used.

The optional *nocoeff* flag allows to read data files with a ImproperCoeff
section for any improper style. Similarly, any improper\_coeff commands
will only be checked for the improper type number and the rest ignored.

Note that the :doc:`improper\_coeff <improper_coeff>` command must be
used for all improper types, though no additional values are
specified.

Restrictions
""""""""""""
 none

**Related commands:** none

:doc:`improper\_style none <improper_none>`

**Default:** none


.. _lws: http://lammps.sandia.gov
.. _ld: Manual.html
.. _lc: Commands_all.html
