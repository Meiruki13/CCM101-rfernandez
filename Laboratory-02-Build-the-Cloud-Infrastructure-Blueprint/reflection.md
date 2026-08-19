# Reflection

Working through this activity gave me a much clearer picture of what
actually happens behind the scenes of a cloud service. Investigating my
KillerCoda environment helped me connect the abstract concepts from Chapter
2 to something concrete — I could see my own compute resource, storage
allocation, and network identity through simple Linux commands.

Of the four infrastructure components, I think compute resources are the
most important, since every other component exists to support running
applications. Without processing power, storage would just be idle data and
networking would have nothing to connect. That said, I also came to
appreciate how dependent these components are on each other — compute needs
storage to persist data and networking to be reachable at all.

Linux plays a foundational role in cloud computing because the majority of
cloud servers run Linux distributions. Its stability, open-source nature,
and strong command-line tools make it ideal for automation and remote
server management — exactly what I experienced navigating KillerCoda purely
through the terminal.

I also learned why technical documentation matters so much before deploying
real infrastructure. If a company migrates to the cloud without documenting
its current environment, it risks miscommunication between engineers, and
later architecture decisions could be based on incomplete information. This
activity's structure — investigate, document, compare, then design — mirrors
what a real cloud engineer would do before proposing an architecture.

New skills I picked up include reading system specifications through the
Linux CLI, comparing equivalent services across AWS, Azure, and GCP, and
building a basic architecture diagram in Draw.io. My GitHub portfolio has
also improved — it now shows a second, more advanced lab building on the
first, demonstrating a progression of both technical skill and
documentation quality.
