#senario 1
# FROM almalinux:9
# ARG course="Devops with AWS" \
#     duration="120hrs"
# RUN echo "Course: $course, duration: $duration"
# CMD ["sleep","100"]

# #senario 2
# ARG version
# FROM almalinux:${version}
# ARG course="Devops with AWS" \
#     duration="120hrs"
# RUN echo "Course: $course, duration: $duration"
# CMD ["sleep","100"]


#senario 3
#when we forgot to send the version setting the default value which can be overrifrn through command line
ARG version
FROM almalinux:${version:-9}
ARG course="Devops with AWS" \
    duration="120hrs"
RUN echo "Course: $course, duration: $duration"
CMD ["sleep","100"]