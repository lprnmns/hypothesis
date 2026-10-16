RELEASE_TYPE: patch

The ``.seed()`` method of :func:`~hypothesis.strategies.randoms` now accepts a
:class:`bytearray`, like :meth:`random.Random.seed`. Previously, it raised
``TypeError: unhashable type: 'bytearray'`` unless ``use_true_random=True``.
