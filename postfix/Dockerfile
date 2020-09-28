FROM alpine:3.12


RUN apk add --no-cache postfix
RUN mkdir /var/mail/domains
RUN chown vmail:postdrop /var/mail/domains

EXPOSE 25 465 587

ENTRYPOINT ["/usr/sbin/postfix"]
CMD ["start-fg"]