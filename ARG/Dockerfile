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

# #senario 3
#sending the arg values through command line
# FROM almalinux:9
# ARG course
# ARG duration
# RUN echo "Course: $course, duration: $duration"
# CMD ["sleep","100"]

#docker build -t arg:v1 --build-arg course=docker .




# #senario 4
# #when we forgot to send the version setting the default value which can be overriden through command line
# ARG version
# FROM almalinux:${version:-9}
# ARG course="Devops with AWS" \
#     duration="120hrs"
# RUN echo "Course: $course, duration: $duration, version: $version"
# CMD ["sleep","100"]


#senario 5
#How can i access ARG values inside container?
#Create a ENV variable and set the value of ARG to that ENV variable
ARG version
FROM almalinux:${version:-9}
ARG course="Devops with AWS" \
    duration="120hrs"
ENV duration=$duration
RUN echo "Course: $course, duration: $duration, version: $version"
CMD ["sleep","100"]


