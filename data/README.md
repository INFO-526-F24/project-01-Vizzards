
# Data

-   **RT IOT 2022**: The dataset consists of 123,117 rows and 77
    columns, capturing detailed network traffic flow data. Key features
    include network identifiers for originating and responding ports,
    protocol and service information (e.g., MQTT), and traffic
    statistics such as packet counts, rates, and header sizes. It also
    tracks flow characteristics (e.g., duration, flags), attack types,
    and payload sizes, which increase during attacks. Additionally,
    bandwidth metrics highlight data flow variations during events like
    DDoS attacks, while inter-arrival times and idle vs. active states
    help analyze IoT device behavior. This dataset is valuable for
    studying network behavior and identifying cyberattacks.

# Codebook for RT IOT 2022 Dataset

RStudio

## Variable Names and Descriptions:

-   **id.orig_p:** The originating port ID, identifying the port from
    which the traffic originates.
-   **id.resp_p:** The responding port ID, identifying the port
    receiving the traffic.
-   **proto:** The protocol used in the communication, such as TCP or
    UDP.
-   **service:** The service in use, such as MQTT, indicating the type
    of application-layer service.
-   **flow_duration:** The duration of the traffic flow in seconds,
    representing the time interval between the first and last packets in
    a session.
-   **fwd_pkts_tot:** The total number of packets forwarded from the
    source to the destination during the flow.
-   **bwd_pkts_tot:** The total number of packets sent back from the
    destination to the source.
-   **fwd_data_pkts_tot:** The total number of data packets forwarded
    from the source.
-   **bwd_data_pkts_tot:** The total number of data packets sent back to
    the source.
-   **fwd_pkts_per_sec:** The number of packets forwarded per second
    from the source.
-   **bwd_pkts_per_sec:** The number of packets sent back per second
    from the destination.
-   **flow_pkts_per_sec:** The total number of packets per second for
    the entire flow, combining forward and backward traffic.
-   **flow_FIN_flag_count:** The number of FIN (finish) flags observed,
    indicating connection termination attempts.
-   **flow_SYN_flag_count:** The number of SYN (synchronize) flags,
    marking the initiation of a connection.
-   **flow_RST_flag_count:** The number of RST (reset) flags, indicating
    an abnormal connection termination.
-   **flow_ACK_flag_count:** The number of ACK (acknowledgment) flags,
    confirming successful packet receipt.
-   **fwd_pkts_payload.min:** The minimum size of the payload in the
    forwarded packets.
-   **fwd_pkts_payload.max:** The maximum size of the payload in the
    forwarded packets.
-   **fwd_pkts_payload.avg:** The average size of the payload in the
    forwarded packets.
-   **fwd_iat.min:** The minimum inter-arrival time between forwarded
    packets.
-   **fwd_iat.avg:** The average inter-arrival time between forwarded
    packets.
-   **flow_iat.min:** The minimum inter-arrival time for the entire flow
    (both forward and backward packets).
-   **active.avg:** The average time the IoT device spends actively
    forwarding traffic.
-   **idle.avg:** The average idle time when the IoT device is not
    forwarding traffic.

## Data Types:

-   **id.orig_p:** Integer
-   **id.resp_p:** Integer
-   **proto:** String
-   **service:** String
-   **flow_duration:** Float
-   **fwd_pkts_tot:** Float
-   **bwd_pkts_tot:** Float
-   **fwd_data_pkts_tot:** Float
-   **bwd_data_pkts_tot:** Float
-   **fwd_pkts_per_sec:** Float
-   **bwd_pkts_per_sec:** Float
-   **flow_pkts_per_sec:** Float
-   **flow_FIN_flag_count:** Integer
-   **flow_SYN_flag_count:** Integer
-   **flow_RST_flag_count:** Integer
-   **flow_ACK_flag_count:** Integer
-   **fwd_pkts_payload.min:** Float
-   **fwd_pkts_payload.max:** Float
-   **fwd_pkts_payload.avg:** Float
-   **fwd_iat.min:** Float
-   **fwd_iat.avg:** Float
-   **flow_iat.min:** Float
-   **active.avg:** Float
-   **idle.avg:** Float
