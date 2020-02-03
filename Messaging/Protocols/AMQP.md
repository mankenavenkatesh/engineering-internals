AMQP in a Nutshell
AMQP, which stands for Advanced Message Queuing Protocol, was designed as an open replacement for existing proprietary messaging middleware. Two of the most important reasons to use AMQP are reliability and interoperability. As the name implies, it provides a wide range of features related to messaging, including reliable queuing, topic-based publish-and-subscribe messaging, flexible routing, transactions, and security. AMQP exchanges route messages directly—in fanout form, by topic, and also based on headers.

There’s a lot of fine-grained control possible with such a rich feature set. You can restrict access to queues, manage their depth, and more. Features like message properties, annotations and headers make it a good fit for a wide range of enterprise applications. This protocol was designed for reliability at the many large companies who depend on messaging to integrate applications and move data around their organisation. In the case of RabbitMQ, there are many different language implementations and great samples available, making it a good choice for building large scale, reliable, resilient, or clustered messaging infrastructures.

AMQP is a binary wire protocol which was designed for interoperability between different vendors. Where other protocols have failed, AMQP adoption has been strong. Companies like JP Morgan use it to process 1 billion messages a day. NASA uses it for Nebula Cloud Computing. Google uses it for complex event processing. Here are a couple of additional AMQP examples and links:

It is used in one of the world’s largest biometric databases India’s Aadhar project—home to 1.2 billion identities.
It is used in the Ocean Observatories Initiative—an architecture that collects 8 terabytes of data per day.
More examples and links are available at amqp.org.


Reasons to use AMQP
- reliability
- interoperability


References 
- https://spring.io/blog/2010/06/14/understanding-amqp-the-protocol-used-by-rabbitmq/
- http://www.amqp.org/
- https://www.rfwireless-world.com/Terminology/AMQP-architecture.html