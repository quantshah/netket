(netket_operator_api)=
# netket.operator

```{eval-rst}
.. currentmodule:: netket.operator

```

The Operator module defines the common interfaces used to interact with quantum operators and super-operators, as well as several concrete implementations of different operators such as netket.hilbert.LocalOperator, netket.hilbert.Ising and others.

NetKet’s operators are all sub-classes of the abstract class netket.hilbert.AbstractOperator, which defines a small set of API respected by all implementations. The inheritance diagram for the class hierarchy of the Operators included with NetKet is shown below (you can click on the nodes in the graph to go to their API documentation page). Dashed nodes represent abstract classes that cannot be instantiated, while the others are concrete and they can be instantiated.



```{eval-rst}
.. inheritance-diagram:: netket.operator netket.experimental.operator
   :top-classes: netket.operator.AbstractOperator
   :parts: 1

```

## Abstract Classes

Below you find a list of all public classes defined in this module
Those classes cannot be directly instantiated, but you can inherit from one of them if you want to define new hilbert spaces.

```{eval-rst}
.. currentmodule:: netket.operator

.. autosummary::
   :toctree: _generated/operator
   :nosignatures:

   AbstractOperator
   AbstractSuperOperator
   DiscreteOperator
   ContinuousOperator
```

## Concrete Classes

Below you find a list of all concrete Operators that you can create on [DiscreteHilbert](netket.hilbert.DiscreteHilbert) spaces.

```{eval-rst}
.. currentmodule:: netket.operator

.. autosummary::
   :toctree: _generated/operator
   :nosignatures:

   BoseHubbard
   GraphOperator
   LocalOperator
   Ising
   Heisenberg
   PauliStrings
   LocalLiouvillian

```

In the experimental submodule there is also a class to represent fermionic operators.

```{eval-rst}
.. currentmodule:: netket

.. autosummary::
   :toctree: _generated/operator
   :nosignatures:

   experimental.operator.FermionOperator2nd
```

### Continuous space operators

This is a list of operators that you can define on [ContinuousHilbert](netket.hilbert.ContinuousHilbert) spaces.

```{eval-rst}
.. currentmodule:: netket.operator

.. autosummary::
   :toctree: _generated/operator
   :nosignatures:

   KineticEnergy
   PotentialEnergy
   SumOperator
```


## Pre-defined operators

Those are easy-to-use constructors for a [LocalOperator](netket.operator.LocalOperator).

```{eval-rst}
.. currentmodule:: netket.operator

.. autosummary::
   :toctree: _generated/operator
   :nosignatures:

   boson.create
   boson.destroy
   boson.number
   boson.proj
   spin.sigmax
   spin.sigmay
   spin.sigmaz
   spin.sigmap
   spin.sigmam

```

In the experimental submodule there are also easy-to-use constructors for common [FermionOperator2nd](netket.experimental.operator.FermionOperator2nd).

```{eval-rst}
.. currentmodule:: netket

.. autosummary::
   :toctree: _generated/operator
   :nosignatures:

   experimental.operator.fermion.create
   experimental.operator.fermion.destroy
   experimental.operator.fermion.number
```
