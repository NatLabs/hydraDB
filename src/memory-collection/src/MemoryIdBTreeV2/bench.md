#### Initial Id BTree
Comparing RBTree, BTree and B+Tree (BpTree)

Benchmarking the performance with 10k entries


Instructions

|                            |      insert() |       get() |   replace() |  entries() |      remove() |
| :------------------------- | ------------: | ----------: | ----------: | ---------: | ------------: |
| B+Tree                     |   175_383_943 | 144_101_415 | 154_390_977 |  4_851_558 |   184_602_693 |
| MotokoStableBTree          |   807_443_679 |   3_564_997 | 807_444_791 |     11_835 |     2_817_599 |
| Memory B+Tree (order 4)    | 1_055_086_701 | 689_991_685 | 718_734_816 | 54_899_157 | 1_226_047_246 |
| Memory B+Tree (order 32)   |   642_321_343 | 478_708_506 | 507_353_186 | 51_104_517 |   690_432_539 |
| Memory B+Tree (order 64)   |   616_553_037 | 466_975_566 | 495_617_480 | 50_834_266 |   650_600_376 |
| Memory B+Tree (order 128)  |   578_034_060 | 425_390_702 | 454_034_399 | 50_698_025 |   592_902_831 |
| Memory B+Tree (order 256)  |   586_513_044 | 422_632_156 | 451_278_853 | 50_628_655 |   589_813_542 |
| Memory B+Tree (order 512)  |   616_811_108 | 420_304_249 | 448_922_929 | 50_592_499 |   611_112_686 |
| Memory B+Tree (order 1024) |   684_994_774 | 417_447_672 | 446_051_586 | 50_578_476 |   663_878_002 |
| Memory B+Tree (order 2048) |   813_134_082 | 413_532_813 | 442_123_510 | 50_578_241 |   776_781_417 |
| Memory B+Tree (order 4096) | 1_044_899_852 | 406_255_727 | 434_846_641 | 50_593_844 |   994_976_782 |


Heap

|                            |    insert() |       get() |   replace() | entries() |    remove() |
| :------------------------- | ----------: | ----------: | ----------: | --------: | ----------: |
| B+Tree                     |     730_052 |     208_960 |     608_964 |     9_084 |     208_964 |
| MotokoStableBTree          |  15_910_668 |       8_960 | -15_468_572 |     9_424 |       8_964 |
| Memory B+Tree (order 4)    |  10_392_744 |   9_234_784 | -22_463_604 | 1_289_552 |  13_697_672 |
| Memory B+Tree (order 32)   |  10_728_940 | -22_646_876 |   8_156_052 | 1_289_360 |  13_242_512 |
| Memory B+Tree (order 64)   | -19_306_468 |   7_324_692 |   7_964_696 | 1_289_360 | -14_905_396 |
| Memory B+Tree (order 128)  |  17_762_452 | -25_406_104 |   7_571_936 | 1_289_328 | -10_848_916 |
| Memory B+Tree (order 256)  |  27_518_908 | -25_440_048 |   7_537_924 | 1_289_328 |  -2_894_912 |
| Memory B+Tree (order 512)  |  14_740_924 | -23_289_508 |   7_513_152 | 1_289_328 |  12_068_456 |
| Memory B+Tree (order 1024) | -11_919_744 |   6_839_048 |   7_479_052 | 1_289_328 | -20_541_184 |
| Memory B+Tree (order 2048) |  24_598_628 | -25_551_904 |   7_425_900 | 1_289_328 |   9_427_588 |
| Memory B+Tree (order 4096) | -18_368_024 |   6_673_120 |   7_313_124 | 1_289_368 |  -5_271_460 |

#### Updated


Instructions

|                            |    insert() |       get() |   replace() |  entries() |      remove() |
| :------------------------- | ----------: | ----------: | ----------: | ---------: | ------------: |
| B+Tree                     | 175_383_943 | 144_101_415 | 154_390_977 |  4_851_558 |   184_602_693 |
| MotokoStableBTree          | 807_443_679 |   3_564_997 | 807_444_791 |     11_835 |     2_817_599 |
| Memory B+Tree (order 4)    | 872_667_810 | 640_728_910 | 961_841_824 | 48_674_343 | 1_065_621_728 |
| Memory B+Tree (order 32)   | 533_884_635 | 430_597_102 | 534_025_016 | 44_683_690 |   619_948_353 |
| Memory B+Tree (order 64)   | 510_189_742 | 421_066_659 | 524_486_573 | 44_399_399 |   586_333_958 |
| Memory B+Tree (order 128)  | 473_103_653 | 380_909_944 | 448_066_641 | 44_256_110 |   535_929_291 |
| Memory B+Tree (order 256)  | 469_107_989 | 379_061_902 | 446_218_582 | 44_183_035 |   525_791_750 |
| Memory B+Tree (order 512)  | 475_816_974 | 377_614_089 | 444_771_003 | 44_144_864 |   527_940_495 |
| Memory B+Tree (order 1024) | 497_487_122 | 375_741_172 | 442_898_086 | 44_129_801 |   542_406_996 |
| Memory B+Tree (order 2048) | 539_784_301 | 372_972_544 | 440_129_458 | 44_129_046 |   577_156_229 |
| Memory B+Tree (order 4096) | 618_032_180 | 367_340_975 | 434_497_889 | 44_144_389 |   646_794_628 |


Heap

|                            |    insert() |       get() |   replace() | entries() |    remove() |
| :------------------------- | ----------: | ----------: | ----------: | --------: | ----------: |
| B+Tree                     |     730_052 |     208_960 |     608_964 |     9_084 |     208_964 |
| MotokoStableBTree          |  15_914_780 |       8_960 | -15_465_184 |     9_424 |       8_964 |
| Memory B+Tree (order 4)    |   5_979_276 |   5_804_864 |   6_204_868 |   889_552 | -22_835_728 |
| Memory B+Tree (order 32)   |   5_646_080 |   4_431_008 |   4_831_012 |   889_360 |   8_467_804 |
| Memory B+Tree (order 64)   | -23_734_788 |   4_326_632 |   4_726_636 |   889_360 |   9_128_972 |
| Memory B+Tree (order 128)  |   8_034_444 | -28_294_092 |   4_439_676 |   889_328 |  10_473_284 |
| Memory B+Tree (order 256)  |  11_526_928 | -26_138_104 |   4_421_124 |   889_328 |  13_306_428 |
| Memory B+Tree (order 512)  | -13_723_024 |   4_007_608 |   4_407_612 |   889_328 | -10_645_604 |
| Memory B+Tree (order 1024) |     174_064 |   3_989_008 |   4_389_012 |   889_328 |   1_094_708 |
| Memory B+Tree (order 2048) |  -5_754_932 |   3_960_016 |   4_360_020 |   889_328 |  -9_374_616 |
| Memory B+Tree (order 4096) |   6_016_540 |   3_898_480 |   4_298_484 |   889_328 |     501_460 |