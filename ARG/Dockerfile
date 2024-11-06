#senario 1
# FROM almalinux:9
# ARG course="Devops with AWS" \
#     duration="120hrs"
# RUN echo "Course: $course, duration: $duration"
# CMD ["sleep","100"]

#senario 2
ARG version
FROM almalinux:${version}
ARG course="Devops with AWS" \
    duration="120hrs"
RUN echo "Course: $course, duration: $duration"
CMD ["sleep","100"]