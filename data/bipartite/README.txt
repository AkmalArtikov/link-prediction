- The simple algorithm improvment is to make global repulsive forses only between groups. So, the nodes from the same group will not interact with each other. It will help to consentrate more nodes around the same interest.

Movielens experiment have shown the following growth in accuracy.
The speed is higher than simple sfdp.

5%                                           (movielens)  (frwiki) , (condmat)        (crime)
sfdp_layout(g)                                : 0.841    , 0.757   ,  0.765,         , 0.569
sfdp_layout(g, groups=groups)                 : 0.814    , 0.724   ,  0.606,         , 0.370
sfdp_layout(g, groups=groups, bipartite=True) : 0.887    , 0.847   ,  0.646,         , 0.452
PA                                            : 0.902    , 0.845   ,  0.597,         , 0.766
NMF(10)                                       : 0.925    , 0.749   ,  0.567,         , 0.552
SVDS(30)                                      : 0.943    , 0.690   ,  0.671,         , 0.568


# Cross validation test 5%

## Crime:
svds-30 : 0.55 (+/- 0.05)
NMF-10 : 0.47 (+/- 0.05)
sfdp-bipartite-simple : 0.32 (+/- 0.07)
PA : 0.39 (+/- 0.09)
sfdp-default : 0.61 (+/- 0.12)


## Movielens:
svds-30 : 0.94 (+/- 0.00)
NMF-10 : 0.93 (+/- 0.00)
sfdp-bipartite-simple : 0.89 (+/- 0.00)
PA : 0.90 (+/- 0.00)
sfdp-default : 0.84 (+/- 0.00)


## Condmat:
svds-30 : 0.66 (+/- 0.02)
NMF-10 : 0.57 (+/- 0.01)
sfdp-bipartite-simple : 0.66 (+/- 0.01)
PA : 0.59 (+/- 0.01)
sfdp-default : 0.76 (+/- 0.01)

## Frwiki:
svds-30 : 0.70 (+/- 0.01)
NMF-10 : 0.74 (+/- 0.01)
sfdp-bipartite-simple : 0.85 (+/- 0.01)
PA : 0.85 (+/- 0.01)
sfdp-default : 0.76 (+/- 0.02)


# Cross validation test 10%

## Crime:
svds-30 : 0.56 (+/- 0.06)
NMF-10 : 0.44 (+/- 0.08)
sfdp-bipartite-simple : 0.36 (+/- 0.11)
PA : 0.37 (+/- 0.10)
sfdp-default : 0.57 (+/- 0.04)


## Movielens:
svds-30 : 0.94 (+/- 0.00)
NMF-10 : 0.93 (+/- 0.00)
sfdp-bipartite-simple : 0.89 (+/- 0.00)
PA : 0.90 (+/- 0.00)
sfdp-default : 0.84 (+/- 0.00)

## Condmat:
svds-30 : 0.66 (+/- 0.01)
NMF-10 : 0.58 (+/- 0.01)
sfdp-bipartite-simple : 0.65 (+/- 0.01)
PA : 0.59 (+/- 0.01)
sfdp-default : 0.75 (+/- 0.01)

## Frwiki:
svds-30 : 0.69 (+/- 0.01)
NMF-10 : 0.74 (+/- 0.02)
sfdp-bipartite-simple : 0.84 (+/- 0.01)
PA : 0.84 (+/- 0.01)
sfdp-default : 0.76 (+/- 0.01)


# Cross validation test 20%

## Crime:
svds-30 : 0.56 (+/- 0.04)
NMF-10 : 0.49 (+/- 0.02)
sfdp-bipartite-simple : 0.41 (+/- 0.03)
PA : 0.41 (+/- 0.04)
sfdp-default : 0.55 (+/- 0.02)

## Movielens:
svds-30 : 0.94 (+/- 0.00)
NMF-10 : 0.93 (+/- 0.00)
sfdp-bipartite-simple : 0.89 (+/- 0.00)
PA : 0.90 (+/- 0.00)
sfdp-default : 0.84 (+/- 0.00)

## Condmat:

## Frwiki:


# Cross validation test 40%

## Crime:
svds-30 : 0.53 (+/- 0.03)
NMF-10 : 0.51 (+/- 0.01)
sfdp-bipartite-simple : 0.48 (+/- 0.03)
PA : 0.44 (+/- 0.02)
sfdp-default : 0.53 (+/- 0.04)
## Movielens:
svds-30 : 0.94 (+/- 0.00)
NMF-10 : 0.92 (+/- 0.00)
sfdp-bipartite-simple : 0.89 (+/- 0.00)
PA : 0.90 (+/- 0.00)
sfdp-default : 0.84 (+/- 0.01)
## Frwiki:
svds-30 : 0.58 (+/- 0.01)
NMF-10 : 0.69 (+/- 0.02)
sfdp-bipartite-simple : 0.79 (+/- 0.01)
PA : 0.79 (+/- 0.00)
sfdp-default : 0.73 (+/- 0.01)
## Condmat:
svds-30 : 0.64 (+/- 0.01)
NMF-10 : 0.58 (+/- 0.01)
sfdp-bipartite-simple : 0.59 (+/- 0.00)
PA : 0.56 (+/- 0.00)
sfdp-default : 0.67 (+/- 0.00)
